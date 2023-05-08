# Comparing `tmp/bioregistry-0.9.7.tar.gz` & `tmp/bioregistry-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioregistry-0.9.7.tar", last modified: Sun May  7 01:27:33 2023, max compression
+gzip compressed data, was "bioregistry-0.9.8.tar", last modified: Mon May  8 01:19:11 2023, max compression
```

## Comparing `bioregistry-0.9.7.tar` & `bioregistry-0.9.8.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-07 00:50:30.000000 bioregistry-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-07 00:50:30.000000 bioregistry-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-07 01:27:33.807938 bioregistry-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-07 00:50:30.000000 bioregistry-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.715937 bioregistry-0.9.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/bulk_prefix_request_template.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.719937 bioregistry-0.9.7/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-07 01:13:48.000000 bioregistry-0.9.7/docs/img/bibliography_years.svg
--rw-r--r--   0 runner    (1001) docker     (123)   157010 2023-05-07 01:14:08.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage.svg
--rw-r--r--   0 runner    (1001) docker     (123)   107004 2023-05-07 01:14:07.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage_bar.svg
--rw-r--r--   0 runner    (1001) docker     (123)    84710 2023-05-07 01:14:08.000000 bioregistry-0.9.7/docs/img/bioregistry_coverage_bar_short.svg
--rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/img/datamodel_umls.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1382043 2023-05-07 01:18:05.000000 bioregistry-0.9.7/docs/img/external_overlap.svg
--rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-07 01:14:35.000000 bioregistry-0.9.7/docs/img/has_attribute.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-07 01:18:06.000000 bioregistry-0.9.7/docs/img/providers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-05-07 01:18:07.000000 bioregistry-0.9.7/docs/img/regex_report.svg
--rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-07 01:14:06.000000 bioregistry-0.9.7/docs/img/xrefs.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.719937 bioregistry-0.9.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/alignment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-07 01:27:22.000000 bioregistry-0.9.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/pandas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-07 00:50:30.000000 bioregistry-0.9.7/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-07 00:50:30.000000 bioregistry-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-07 01:27:33.811938 bioregistry-0.9.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.707937 bioregistry-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.723937 bioregistry-0.9.7/src/bioregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/align/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/analysis/title_tfidf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/app/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.727937 bioregistry-0.9.7/src/bioregistry/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/collections.html
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/context.html
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contexts.html
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contributor.html
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/contributors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/keywords.html
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/owners.html
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/relations.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/highlights/twitter.html
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/access.html
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/acknowledgements.html
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/download.html
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/related.html
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/meta/sustainability.html
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/metaresource.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/metaresources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/prose.html
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/reference.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.731938 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_providers.html
--rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resource.html
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/templates/resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/app/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.735937 bioregistry-0.9.7/src/bioregistry/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/curie_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/curie_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/benchmarks/uri_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/bibliometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.735937 bioregistry-0.9.7/src/bioregistry/curation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_co_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_descriptions_from_gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_javert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/add_ontology_regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_name_suffixes.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/clean_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/cleanup_authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/deprecation_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/enrich_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/import_pc_semiautomatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/make_description_curation_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/map_bartoc_via_wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/map_re3data_via_fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/rename_metaprefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/review_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/suggest_author_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/curation/suggest_uniprot_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.743938 bioregistry-0.9.7/src/bioregistry/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4590847 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/bioregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/collections.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/contexts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.711937 bioregistry-0.9.7/src/bioregistry/data/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.743938 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/
--rw-r--r--   0 runner    (1001) docker     (123)   302996 2023-05-07 00:57:27.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   623964 2023-05-07 00:57:27.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1281529 2023-05-07 00:57:20.000000 bioregistry-0.9.7/src/bioregistry/data/external/aberowl/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.751938 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/
--rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-07 00:53:01.000000 bioregistry-0.9.7/src/bioregistry/data/external/agroportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.755938 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/
--rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-07 00:53:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-07 00:53:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/bartoc/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-07 01:05:06.000000 bioregistry-0.9.7/src/bioregistry/data/external/biocontext/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-07 00:53:19.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-07 00:53:18.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   355095 2023-05-07 00:53:17.000000 bioregistry-0.9.7/src/bioregistry/data/external/biolink/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.759938 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/
--rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-07 00:57:10.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   606737 2023-05-07 00:57:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  3539154 2023-05-07 00:57:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/bioportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-07 00:53:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/raw.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cheminf/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-07 01:05:04.000000 bioregistry-0.9.7/src/bioregistry/data/external/cheminf/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-07 01:05:00.000000 bioregistry-0.9.7/src/bioregistry/data/external/cropoct/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-07 01:04:57.000000 bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/edam/
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-07 00:53:15.000000 bioregistry-0.9.7/src/bioregistry/data/external/edam/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-07 00:53:14.000000 bioregistry-0.9.7/src/bioregistry/data/external/edam/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.767938 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   253879 2023-05-07 01:11:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   745109 2023-05-07 01:11:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/go/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-07 00:57:13.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-07 00:57:12.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-07 00:57:12.000000 bioregistry-0.9.7/src/bioregistry/data/external/go/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-07 01:04:45.000000 bioregistry-0.9.7/src/bioregistry/data/external/hl7/curation.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.771938 bioregistry-0.9.7/src/bioregistry/data/external/miriam/
--rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-07 01:04:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/miriam/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-07 01:04:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/miriam/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.775938 bioregistry-0.9.7/src/bioregistry/data/external/n2t/
--rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-07 01:05:15.000000 bioregistry-0.9.7/src/bioregistry/data/external/n2t/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1279133 2023-05-07 01:05:09.000000 bioregistry-0.9.7/src/bioregistry/data/external/n2t/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-07 01:04:43.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-07 01:04:42.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-07 01:04:42.000000 bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/
--rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-07 00:51:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-07 00:51:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.779938 bioregistry-0.9.7/src/bioregistry/data/external/ols/
--rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-07 01:11:49.000000 bioregistry-0.9.7/src/bioregistry/data/external/ols/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-07 01:11:49.000000 bioregistry-0.9.7/src/bioregistry/data/external/ols/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.783938 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-07 01:04:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/ontobee/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.783938 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/
--rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-07 00:57:31.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-07 00:57:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-07 00:57:30.000000 bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/raw.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.787938 bioregistry-0.9.7/src/bioregistry/data/external/re3data/
--rw-r--r--   0 runner    (1001) docker     (123)  1742778 2023-05-07 01:04:33.000000 bioregistry-0.9.7/src/bioregistry/data/external/re3data/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2439371 2023-05-07 01:04:32.000000 bioregistry-0.9.7/src/bioregistry/data/external/re3data/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.791938 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-07 01:11:40.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    67268 2023-05-07 01:11:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-05-07 01:11:39.000000 bioregistry-0.9.7/src/bioregistry/data/external/uniprot/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.791938 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-07 01:11:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-07 01:11:36.000000 bioregistry-0.9.7/src/bioregistry/data/external/wikidata/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/metaregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-07 01:11:50.000000 bioregistry-0.9.7/src/bioregistry/data/mismatch.json
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_biolink.json
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_go.json
--rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_ols.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/data/processing_wikidata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.795938 bioregistry-0.9.7/src/bioregistry/export/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/prefix_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/rdf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/schema_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/sssom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/tables_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/tsv_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/warnings_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/export/yaml_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/external/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/go.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/hl7/OID_Report.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/hl7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/external/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.799938 bioregistry-0.9.7/src/bioregistry/gh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/gh/new_prefix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.803938 bioregistry-0.9.7/src/bioregistry/health/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/check_homepages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/check_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/health/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/license_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/metaresource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/parse_iri.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/record_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resolve_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.803938 bioregistry-0.9.7/src/bioregistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)   106540 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/upload_ndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/uri_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-07 00:50:30.000000 bioregistry-0.9.7/src/bioregistry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-07 01:27:22.000000 bioregistry-0.9.7/src/bioregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.723937 bioregistry-0.9.7/src/bioregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:50:47.000000 bioregistry-0.9.7/src/bioregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 01:27:33.000000 bioregistry-0.9.7/src/bioregistry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_identifiers_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_indra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_metaregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_usages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:27:33.807938 bioregistry-0.9.7/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-07 00:50:30.000000 bioregistry-0.9.7/tests/test_web/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.410652 bioregistry-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-08 00:45:09.000000 bioregistry-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-08 00:45:09.000000 bioregistry-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-08 01:19:11.410652 bioregistry-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-08 00:45:09.000000 bioregistry-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.338652 bioregistry-0.9.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/bulk_prefix_request_template.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.342652 bioregistry-0.9.8/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-08 01:06:55.000000 bioregistry-0.9.8/docs/img/bibliography_years.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   157010 2023-05-08 01:07:12.000000 bioregistry-0.9.8/docs/img/bioregistry_coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   107004 2023-05-08 01:07:12.000000 bioregistry-0.9.8/docs/img/bioregistry_coverage_bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    84710 2023-05-08 01:07:13.000000 bioregistry-0.9.8/docs/img/bioregistry_coverage_bar_short.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/img/datamodel_umls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1382043 2023-05-08 01:10:44.000000 bioregistry-0.9.8/docs/img/external_overlap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-08 01:07:37.000000 bioregistry-0.9.8/docs/img/has_attribute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-08 01:10:45.000000 bioregistry-0.9.8/docs/img/providers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22283 2023-05-08 01:10:46.000000 bioregistry-0.9.8/docs/img/regex_report.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-08 01:07:11.000000 bioregistry-0.9.8/docs/img/xrefs.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.342652 bioregistry-0.9.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-08 01:19:01.000000 bioregistry-0.9.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-08 00:45:09.000000 bioregistry-0.9.8/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-08 00:45:09.000000 bioregistry-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-08 01:19:11.410652 bioregistry-0.9.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.334652 bioregistry-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.346652 bioregistry-0.9.8/src/bioregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.350652 bioregistry-0.9.8/src/bioregistry/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/align/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.350652 bioregistry-0.9.8/src/bioregistry/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/analysis/title_tfidf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.350652 bioregistry-0.9.8/src/bioregistry/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.350652 bioregistry-0.9.8/src/bioregistry/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.354652 bioregistry-0.9.8/src/bioregistry/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/collections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/context.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/contexts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/contributor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/contributors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.354652 bioregistry-0.9.8/src/bioregistry/app/templates/highlights/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/highlights/keywords.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/highlights/owners.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/highlights/relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/highlights/twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.354652 bioregistry-0.9.8/src/bioregistry/app/templates/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/access.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/acknowledgements.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/related.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/meta/sustainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/metaresource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/metaresources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/prose.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/reference.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.354652 bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/missing_providers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/templates/resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/app/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.354652 bioregistry-0.9.8/src/bioregistry/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/curie_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/curie_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/benchmarks/uri_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/bibliometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.358652 bioregistry-0.9.8/src/bioregistry/curation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_co_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_descriptions_from_gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_examples_from_javert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_examples_from_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/add_ontology_regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/clean_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/clean_name_suffixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/clean_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/cleanup_authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/deprecation_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/enrich_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/import_pc_semiautomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/make_description_curation_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/map_bartoc_via_wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/map_re3data_via_fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/rename_metaprefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/review_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/suggest_author_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/curation/suggest_uniprot_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.366652 bioregistry-0.9.8/src/bioregistry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4590847 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/bioregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/collections.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/contexts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.334652 bioregistry-0.9.8/src/bioregistry/data/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.366652 bioregistry-0.9.8/src/bioregistry/data/external/aberowl/
+-rw-r--r--   0 runner    (1001) docker     (123)   302996 2023-05-08 01:05:09.000000 bioregistry-0.9.8/src/bioregistry/data/external/aberowl/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   623964 2023-05-08 01:05:08.000000 bioregistry-0.9.8/src/bioregistry/data/external/aberowl/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1281529 2023-05-08 01:05:03.000000 bioregistry-0.9.8/src/bioregistry/data/external/aberowl/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.366652 bioregistry-0.9.8/src/bioregistry/data/external/agroportal/
+-rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-08 01:01:01.000000 bioregistry-0.9.8/src/bioregistry/data/external/agroportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-08 01:01:01.000000 bioregistry-0.9.8/src/bioregistry/data/external/agroportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-08 01:01:01.000000 bioregistry-0.9.8/src/bioregistry/data/external/agroportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.370652 bioregistry-0.9.8/src/bioregistry/data/external/bartoc/
+-rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-08 00:59:21.000000 bioregistry-0.9.8/src/bioregistry/data/external/bartoc/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-08 00:59:21.000000 bioregistry-0.9.8/src/bioregistry/data/external/bartoc/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.374652 bioregistry-0.9.8/src/bioregistry/data/external/biocontext/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-08 00:59:17.000000 bioregistry-0.9.8/src/bioregistry/data/external/biocontext/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-08 00:59:17.000000 bioregistry-0.9.8/src/bioregistry/data/external/biocontext/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-08 00:59:17.000000 bioregistry-0.9.8/src/bioregistry/data/external/biocontext/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.374652 bioregistry-0.9.8/src/bioregistry/data/external/biolink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-08 01:04:55.000000 bioregistry-0.9.8/src/bioregistry/data/external/biolink/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-08 01:04:55.000000 bioregistry-0.9.8/src/bioregistry/data/external/biolink/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   355095 2023-05-08 01:04:54.000000 bioregistry-0.9.8/src/bioregistry/data/external/biolink/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.374652 bioregistry-0.9.8/src/bioregistry/data/external/bioportal/
+-rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-08 01:04:52.000000 bioregistry-0.9.8/src/bioregistry/data/external/bioportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   606737 2023-05-08 01:04:52.000000 bioregistry-0.9.8/src/bioregistry/data/external/bioportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3539154 2023-05-08 01:04:52.000000 bioregistry-0.9.8/src/bioregistry/data/external/bioportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.378652 bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-08 01:01:04.000000 bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-08 01:01:04.000000 bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-08 01:01:04.000000 bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/raw.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.378652 bioregistry-0.9.8/src/bioregistry/data/external/cheminf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-08 00:52:11.000000 bioregistry-0.9.8/src/bioregistry/data/external/cheminf/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.378652 bioregistry-0.9.8/src/bioregistry/data/external/cropoct/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-08 00:45:55.000000 bioregistry-0.9.8/src/bioregistry/data/external/cropoct/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-08 00:45:55.000000 bioregistry-0.9.8/src/bioregistry/data/external/cropoct/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-08 00:45:54.000000 bioregistry-0.9.8/src/bioregistry/data/external/cropoct/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.378652 bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-08 00:52:45.000000 bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-08 00:52:45.000000 bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-08 00:52:45.000000 bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.378652 bioregistry-0.9.8/src/bioregistry/data/external/edam/
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-08 00:59:27.000000 bioregistry-0.9.8/src/bioregistry/data/external/edam/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-08 00:59:26.000000 bioregistry-0.9.8/src/bioregistry/data/external/edam/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.382652 bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   253879 2023-05-08 00:52:02.000000 bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   745109 2023-05-08 00:52:02.000000 bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.382652 bioregistry-0.9.8/src/bioregistry/data/external/go/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-08 00:59:29.000000 bioregistry-0.9.8/src/bioregistry/data/external/go/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-08 00:59:29.000000 bioregistry-0.9.8/src/bioregistry/data/external/go/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-08 00:59:29.000000 bioregistry-0.9.8/src/bioregistry/data/external/go/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.382652 bioregistry-0.9.8/src/bioregistry/data/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/external/hl7/curation.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.382652 bioregistry-0.9.8/src/bioregistry/data/external/miriam/
+-rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-08 00:52:49.000000 bioregistry-0.9.8/src/bioregistry/data/external/miriam/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-08 00:52:49.000000 bioregistry-0.9.8/src/bioregistry/data/external/miriam/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.386652 bioregistry-0.9.8/src/bioregistry/data/external/n2t/
+-rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-08 00:52:18.000000 bioregistry-0.9.8/src/bioregistry/data/external/n2t/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1279133 2023-05-08 00:52:13.000000 bioregistry-0.9.8/src/bioregistry/data/external/n2t/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.386652 bioregistry-0.9.8/src/bioregistry/data/external/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-08 00:59:36.000000 bioregistry-0.9.8/src/bioregistry/data/external/ncbi/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-08 00:59:35.000000 bioregistry-0.9.8/src/bioregistry/data/external/ncbi/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-08 00:59:35.000000 bioregistry-0.9.8/src/bioregistry/data/external/ncbi/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.386652 bioregistry-0.9.8/src/bioregistry/data/external/obofoundry/
+-rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-08 00:52:21.000000 bioregistry-0.9.8/src/bioregistry/data/external/obofoundry/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-08 00:52:20.000000 bioregistry-0.9.8/src/bioregistry/data/external/obofoundry/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.390652 bioregistry-0.9.8/src/bioregistry/data/external/ols/
+-rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-08 00:52:32.000000 bioregistry-0.9.8/src/bioregistry/data/external/ols/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-08 00:52:32.000000 bioregistry-0.9.8/src/bioregistry/data/external/ols/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.390652 bioregistry-0.9.8/src/bioregistry/data/external/ontobee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-08 00:45:58.000000 bioregistry-0.9.8/src/bioregistry/data/external/ontobee/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-08 00:45:57.000000 bioregistry-0.9.8/src/bioregistry/data/external/ontobee/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-08 00:45:57.000000 bioregistry-0.9.8/src/bioregistry/data/external/ontobee/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.390652 bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/
+-rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-08 00:59:33.000000 bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-08 00:59:32.000000 bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-08 00:59:32.000000 bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/raw.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.394652 bioregistry-0.9.8/src/bioregistry/data/external/re3data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1742778 2023-05-08 00:59:15.000000 bioregistry-0.9.8/src/bioregistry/data/external/re3data/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2439371 2023-05-08 00:59:14.000000 bioregistry-0.9.8/src/bioregistry/data/external/re3data/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.398652 bioregistry-0.9.8/src/bioregistry/data/external/uniprot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-08 00:52:07.000000 bioregistry-0.9.8/src/bioregistry/data/external/uniprot/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    67268 2023-05-08 00:52:06.000000 bioregistry-0.9.8/src/bioregistry/data/external/uniprot/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-05-08 00:52:06.000000 bioregistry-0.9.8/src/bioregistry/data/external/uniprot/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.398652 bioregistry-0.9.8/src/bioregistry/data/external/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-08 00:52:26.000000 bioregistry-0.9.8/src/bioregistry/data/external/wikidata/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-08 00:52:26.000000 bioregistry-0.9.8/src/bioregistry/data/external/wikidata/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/metaregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-08 01:05:11.000000 bioregistry-0.9.8/src/bioregistry/data/mismatch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/processing_biolink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/processing_go.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/processing_ols.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/data/processing_wikidata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.398652 bioregistry-0.9.8/src/bioregistry/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/prefix_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/rdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/schema_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/sssom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/tables_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/tsv_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/warnings_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/export/yaml_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.402652 bioregistry-0.9.8/src/bioregistry/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/go.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.402652 bioregistry-0.9.8/src/bioregistry/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/hl7/OID_Report.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/hl7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/external/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.402652 bioregistry-0.9.8/src/bioregistry/gh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/gh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/gh/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/gh/new_prefix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.406652 bioregistry-0.9.8/src/bioregistry/health/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/health/check_homepages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/health/check_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/health/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/license_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/metaresource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/parse_iri.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/record_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/resolve_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.406652 bioregistry-0.9.8/src/bioregistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)   106540 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/upload_ndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/uri_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-08 00:45:09.000000 bioregistry-0.9.8/src/bioregistry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 01:19:01.000000 bioregistry-0.9.8/src/bioregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.346652 bioregistry-0.9.8/src/bioregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 00:45:19.000000 bioregistry-0.9.8/src/bioregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 01:19:11.000000 bioregistry-0.9.8/src/bioregistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.406652 bioregistry-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_identifiers_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_indra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_metaregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_usages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 01:19:11.410652 bioregistry-0.9.8/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_web/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-08 00:45:09.000000 bioregistry-0.9.8/tests/test_web/test_ui.py
```

### Comparing `bioregistry-0.9.7/LICENSE` & `bioregistry-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/MANIFEST.in` & `bioregistry-0.9.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/PKG-INFO` & `bioregistry-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.7
+Version: 0.9.8
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.7 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.8 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.7/README.md` & `bioregistry-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/docs/bulk_prefix_request_template.tsv` & `bioregistry-0.9.8/docs/bulk_prefix_request_template.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/docs/img/bibliography_years.svg` & `bioregistry-0.9.8/docs/img/bibliography_years.svg`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3133 3a34 382e 3838 3835 3439  T01:13:48.888549
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3036 3a35 352e 3032 3839 3430  T01:06:55.028940
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -78,392 +78,392 @@
 000004d0: 3c70 6174 6820 643d 224d 2034 362e 3238  <path d="M 46.28
 000004e0: 3836 3535 2032 3038 2e39 3938 3731 3420  8655 208.998714 
 000004f0: 0a4c 2036 302e 3033 3738 3939 2032 3038  .L 60.037899 208
 00000500: 2e39 3938 3731 3420 0a4c 2036 302e 3033  .998714 .L 60.03
 00000510: 3738 3939 2032 3038 2e39 3938 3731 3420  7899 208.998714 
 00000520: 0a4c 2034 362e 3238 3836 3535 2032 3038  .L 46.288655 208
 00000530: 2e39 3938 3731 3420 0a7a 0a22 2063 6c69  .998714 .z." cli
-00000540: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-00000550: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+00000540: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+00000550: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 00000560: 3d22 6669 6c6c 3a20 2365 6139 3661 3322  ="fill: #ea96a3"
 00000570: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000580: 2069 643d 2270 6174 6368 5f34 223e 0a20   id="patch_4">. 
 00000590: 2020 203c 7061 7468 2064 3d22 4d20 3633     <path d="M 63
 000005a0: 2e34 3735 3231 2032 3038 2e39 3938 3731  .47521 208.99871
 000005b0: 3420 0a4c 2037 372e 3232 3434 3534 2032  4 .L 77.224454 2
 000005c0: 3038 2e39 3938 3731 3420 0a4c 2037 372e  08.998714 .L 77.
 000005d0: 3232 3434 3534 2032 3033 2e38 3937 3335  224454 203.89735
 000005e0: 200a 4c20 3633 2e34 3735 3231 2032 3033   .L 63.47521 203
 000005f0: 2e38 3937 3335 200a 7a0a 2220 636c 6970  .89735 .z." clip
-00000600: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
-00000610: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
+00000600: 2d70 6174 683d 2275 726c 2823 7032 3462  -path="url(#p24b
+00000610: 3463 3830 6538 3929 2220 7374 796c 653d  4c80e89)" style=
 00000620: 2266 696c 6c3a 2023 6539 3937 3931 222f  "fill: #e99791"/
 00000630: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00000640: 6964 3d22 7061 7463 685f 3522 3e0a 2020  id="patch_5">.  
 00000650: 2020 3c70 6174 6820 643d 224d 2038 302e    <path d="M 80.
 00000660: 3636 3137 3635 2032 3038 2e39 3938 3731  661765 208.99871
 00000670: 3420 0a4c 2039 342e 3431 3130 3038 2032  4 .L 94.411008 2
 00000680: 3038 2e39 3938 3731 3420 0a4c 2039 342e  08.998714 .L 94.
 00000690: 3431 3130 3038 2031 3938 2e37 3935 3938  411008 198.79598
 000006a0: 3520 0a4c 2038 302e 3636 3137 3635 2031  5 .L 80.661765 1
 000006b0: 3938 2e37 3935 3938 3520 0a7a 0a22 2063  98.795985 .z." c
 000006c0: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-000006d0: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
+000006d0: 3234 6234 6338 3065 3839 2922 2073 7479  24b4c80e89)" sty
 000006e0: 6c65 3d22 6669 6c6c 3a20 2365 3539 3437  le="fill: #e5947
 000006f0: 3122 2f3e 0a20 2020 3c2f 673e 0a20 2020  1"/>.   </g>.   
 00000700: 3c67 2069 643d 2270 6174 6368 5f36 223e  <g id="patch_6">
 00000710: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 00000720: 3937 2e38 3438 3331 3920 3230 382e 3939  97.848319 208.99
 00000730: 3837 3134 200a 4c20 3131 312e 3539 3735  8714 .L 111.5975
 00000740: 3633 2032 3038 2e39 3938 3731 3420 0a4c  63 208.998714 .L
 00000750: 2031 3131 2e35 3937 3536 3320 3137 382e   111.597563 178.
 00000760: 3339 3035 3237 200a 4c20 3937 2e38 3438  390527 .L 97.848
 00000770: 3331 3920 3137 382e 3339 3035 3237 200a  319 178.390527 .
 00000780: 7a0a 2220 636c 6970 2d70 6174 683d 2275  z." clip-path="u
-00000790: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
+00000790: 726c 2823 7032 3462 3463 3830 6538 3929  rl(#p24b4c80e89)
 000007a0: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 000007b0: 6437 3934 3465 222f 3e0a 2020 203c 2f67  d7944e"/>.   </g
 000007c0: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 000007d0: 685f 3722 3e0a 2020 2020 3c70 6174 6820  h_7">.    <path 
 000007e0: 643d 224d 2031 3135 2e30 3334 3837 3420  d="M 115.034874 
 000007f0: 3230 382e 3939 3837 3134 200a 4c20 3132  208.998714 .L 12
 00000800: 382e 3738 3431 3137 2032 3038 2e39 3938  8.784117 208.998
 00000810: 3731 3420 0a4c 2031 3238 2e37 3834 3131  714 .L 128.78411
 00000820: 3720 3138 382e 3539 3332 3536 200a 4c20  7 188.593256 .L 
 00000830: 3131 352e 3033 3438 3734 2031 3838 2e35  115.034874 188.5
 00000840: 3933 3235 3620 0a7a 0a22 2063 6c69 702d  93256 .z." clip-
-00000850: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-00000860: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00000850: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+00000860: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 00000870: 6669 6c6c 3a20 2363 3639 3934 6222 2f3e  fill: #c6994b"/>
 00000880: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00000890: 643d 2270 6174 6368 5f38 223e 0a20 2020  d="patch_8">.   
 000008a0: 203c 7061 7468 2064 3d22 4d20 3133 322e   <path d="M 132.
 000008b0: 3232 3134 3238 2032 3038 2e39 3938 3731  221428 208.99871
 000008c0: 3420 0a4c 2031 3435 2e39 3730 3637 3220  4 .L 145.970672 
 000008d0: 3230 382e 3939 3837 3134 200a 4c20 3134  208.998714 .L 14
 000008e0: 352e 3937 3036 3732 2031 3733 2e32 3839  5.970672 173.289
 000008f0: 3136 3220 0a4c 2031 3332 2e32 3231 3432  162 .L 132.22142
 00000900: 3820 3137 332e 3238 3931 3632 200a 7a0a  8 173.289162 .z.
 00000910: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00000920: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
+00000920: 2823 7032 3462 3463 3830 6538 3929 2220  (#p24b4c80e89)" 
 00000930: 7374 796c 653d 2266 696c 6c3a 2023 6238  style="fill: #b8
 00000940: 3963 3439 222f 3e0a 2020 203c 2f67 3e0a  9c49"/>.   </g>.
 00000950: 2020 203c 6720 6964 3d22 7061 7463 685f     <g id="patch_
 00000960: 3922 3e0a 2020 2020 3c70 6174 6820 643d  9">.    <path d=
 00000970: 224d 2031 3439 2e34 3037 3938 3320 3230  "M 149.407983 20
 00000980: 382e 3939 3837 3134 200a 4c20 3136 332e  8.998714 .L 163.
 00000990: 3135 3732 3236 2032 3038 2e39 3938 3731  157226 208.99871
 000009a0: 3420 0a4c 2031 3633 2e31 3537 3232 3620  4 .L 163.157226 
 000009b0: 3135 372e 3938 3530 3639 200a 4c20 3134  157.985069 .L 14
 000009c0: 392e 3430 3739 3833 2031 3537 2e39 3835  9.407983 157.985
 000009d0: 3036 3920 0a7a 0a22 2063 6c69 702d 7061  069 .z." clip-pa
-000009e0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-000009f0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+000009e0: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+000009f0: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 00000a00: 6c6c 3a20 2361 6239 6534 3722 2f3e 0a20  ll: #ab9e47"/>. 
 00000a10: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000a20: 2270 6174 6368 5f31 3022 3e0a 2020 2020  "patch_10">.    
 00000a30: 3c70 6174 6820 643d 224d 2031 3636 2e35  <path d="M 166.5
 00000a40: 3934 3533 3720 3230 382e 3939 3837 3134  94537 208.998714
 00000a50: 200a 4c20 3138 302e 3334 3337 3831 2032   .L 180.343781 2
 00000a60: 3038 2e39 3938 3731 3420 0a4c 2031 3830  08.998714 .L 180
 00000a70: 2e33 3433 3738 3120 3138 332e 3439 3138  .343781 183.4918
 00000a80: 3932 200a 4c20 3136 362e 3539 3435 3337  92 .L 166.594537
 00000a90: 2031 3833 2e34 3931 3839 3220 0a7a 0a22   183.491892 .z."
 00000aa0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00000ab0: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
+00000ab0: 2370 3234 6234 6338 3065 3839 2922 2073  #p24b4c80e89)" s
 00000ac0: 7479 6c65 3d22 6669 6c6c 3a20 2339 6561  tyle="fill: #9ea
 00000ad0: 3034 3522 2f3e 0a20 2020 3c2f 673e 0a20  045"/>.   </g>. 
 00000ae0: 2020 3c67 2069 643d 2270 6174 6368 5f31    <g id="patch_1
 00000af0: 3122 3e0a 2020 2020 3c70 6174 6820 643d  1">.    <path d=
 00000b00: 224d 2031 3833 2e37 3831 3039 3220 3230  "M 183.781092 20
 00000b10: 382e 3939 3837 3134 200a 4c20 3139 372e  8.998714 .L 197.
 00000b20: 3533 3033 3335 2032 3038 2e39 3938 3731  530335 208.99871
 00000b30: 3420 0a4c 2031 3937 2e35 3330 3333 3520  4 .L 197.530335 
 00000b40: 3133 372e 3537 3936 3131 200a 4c20 3138  137.579611 .L 18
 00000b50: 332e 3738 3130 3932 2031 3337 2e35 3739  3.781092 137.579
 00000b60: 3631 3120 0a7a 0a22 2063 6c69 702d 7061  611 .z." clip-pa
-00000b70: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-00000b80: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+00000b70: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+00000b80: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 00000b90: 6c6c 3a20 2339 3161 3434 3622 2f3e 0a20  ll: #91a446"/>. 
 00000ba0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000bb0: 2270 6174 6368 5f31 3222 3e0a 2020 2020  "patch_12">.    
 00000bc0: 3c70 6174 6820 643d 224d 2032 3030 2e39  <path d="M 200.9
 00000bd0: 3637 3634 3620 3230 382e 3939 3837 3134  67646 208.998714
 00000be0: 200a 4c20 3231 342e 3731 3638 3920 3230   .L 214.71689 20
 00000bf0: 382e 3939 3837 3134 200a 4c20 3231 342e  8.998714 .L 214.
 00000c00: 3731 3638 3920 3133 322e 3437 3832 3436  71689 132.478246
 00000c10: 200a 4c20 3230 302e 3936 3736 3436 2031   .L 200.967646 1
 00000c20: 3332 2e34 3738 3234 3620 0a7a 0a22 2063  32.478246 .z." c
 00000c30: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00000c40: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
+00000c40: 3234 6234 6338 3065 3839 2922 2073 7479  24b4c80e89)" sty
 00000c50: 6c65 3d22 6669 6c6c 3a20 2337 6661 3934  le="fill: #7fa94
 00000c60: 3622 2f3e 0a20 2020 3c2f 673e 0a20 2020  6"/>.   </g>.   
 00000c70: 3c67 2069 643d 2270 6174 6368 5f31 3322  <g id="patch_13"
 00000c80: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00000c90: 2032 3138 2e31 3534 3230 3120 3230 382e   218.154201 208.
 00000ca0: 3939 3837 3134 200a 4c20 3233 312e 3930  998714 .L 231.90
 00000cb0: 3334 3435 2032 3038 2e39 3938 3731 3420  3445 208.998714 
 00000cc0: 0a4c 2032 3331 2e39 3033 3434 3520 3335  .L 231.903445 35
 00000cd0: 2e35 3532 3332 200a 4c20 3231 382e 3135  .55232 .L 218.15
 00000ce0: 3432 3031 2033 352e 3535 3233 3220 0a7a  4201 35.55232 .z
 00000cf0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000d00: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+00000d00: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 00000d10: 2073 7479 6c65 3d22 6669 6c6c 3a20 2336   style="fill: #6
 00000d20: 3061 6534 3722 2f3e 0a20 2020 3c2f 673e  0ae47"/>.   </g>
 00000d30: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000d40: 5f31 3422 3e0a 2020 2020 3c70 6174 6820  _14">.    <path 
 00000d50: 643d 224d 2032 3335 2e33 3430 3735 3520  d="M 235.340755 
 00000d60: 3230 382e 3939 3837 3134 200a 4c20 3234  208.998714 .L 24
 00000d70: 392e 3038 3939 3939 2032 3038 2e39 3938  9.089999 208.998
 00000d80: 3731 3420 0a4c 2032 3439 2e30 3839 3939  714 .L 249.08999
 00000d90: 3920 3831 2e34 3634 3630 3120 0a4c 2032  9 81.464601 .L 2
 00000da0: 3335 2e33 3430 3735 3520 3831 2e34 3634  35.340755 81.464
 00000db0: 3630 3120 0a7a 0a22 2063 6c69 702d 7061  601 .z." clip-pa
-00000dc0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-00000dd0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+00000dc0: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+00000dd0: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 00000de0: 6c6c 3a20 2334 3862 3036 6122 2f3e 0a20  ll: #48b06a"/>. 
 00000df0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000e00: 2270 6174 6368 5f31 3522 3e0a 2020 2020  "patch_15">.    
 00000e10: 3c70 6174 6820 643d 224d 2032 3532 2e35  <path d="M 252.5
 00000e20: 3237 3331 2032 3038 2e39 3938 3731 3420  2731 208.998714 
 00000e30: 0a4c 2032 3636 2e32 3736 3535 3420 3230  .L 266.276554 20
 00000e40: 382e 3939 3837 3134 200a 4c20 3236 362e  8.998714 .L 266.
 00000e50: 3237 3635 3534 2034 302e 3635 3336 3834  276554 40.653684
 00000e60: 200a 4c20 3235 322e 3532 3733 3120 3430   .L 252.52731 40
 00000e70: 2e36 3533 3638 3420 0a7a 0a22 2063 6c69  .653684 .z." cli
-00000e80: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-00000e90: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+00000e80: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+00000e90: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 00000ea0: 3d22 6669 6c6c 3a20 2334 3961 6538 3322  ="fill: #49ae83"
 00000eb0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000ec0: 2069 643d 2270 6174 6368 5f31 3622 3e0a   id="patch_16">.
 00000ed0: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
 00000ee0: 3639 2e37 3133 3836 3520 3230 382e 3939  69.713865 208.99
 00000ef0: 3837 3134 200a 4c20 3238 332e 3436 3331  8714 .L 283.4631
 00000f00: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00000f10: 2032 3833 2e34 3633 3130 3820 3631 2e30   283.463108 61.0
 00000f20: 3539 3134 3220 0a4c 2032 3639 2e37 3133  59142 .L 269.713
 00000f30: 3836 3520 3631 2e30 3539 3134 3220 0a7a  865 61.059142 .z
 00000f40: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000f50: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+00000f50: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 00000f60: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 00000f70: 6161 6439 3122 2f3e 0a20 2020 3c2f 673e  aad91"/>.   </g>
 00000f80: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000f90: 5f31 3722 3e0a 2020 2020 3c70 6174 6820  _17">.    <path 
 00000fa0: 643d 224d 2032 3836 2e39 3030 3431 3920  d="M 286.900419 
 00000fb0: 3230 382e 3939 3837 3134 200a 4c20 3330  208.998714 .L 30
 00000fc0: 302e 3634 3936 3633 2032 3038 2e39 3938  0.649663 208.998
 00000fd0: 3731 3420 0a4c 2033 3030 2e36 3439 3636  714 .L 300.64966
 00000fe0: 3320 3335 2e35 3532 3332 200a 4c20 3238  3 35.55232 .L 28
 00000ff0: 362e 3930 3034 3139 2033 352e 3535 3233  6.900419 35.5523
 00001000: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001010: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
-00001020: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
+00001010: 3d22 7572 6c28 2370 3234 6234 6338 3065  ="url(#p24b4c80e
+00001020: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 00001030: 3a20 2334 6161 6339 6222 2f3e 0a20 2020  : #4aac9b"/>.   
 00001040: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001050: 6174 6368 5f31 3822 3e0a 2020 2020 3c70  atch_18">.    <p
 00001060: 6174 6820 643d 224d 2033 3034 2e30 3836  ath d="M 304.086
 00001070: 3937 3420 3230 382e 3939 3837 3134 200a  974 208.998714 .
 00001080: 4c20 3331 372e 3833 3632 3137 2032 3038  L 317.836217 208
 00001090: 2e39 3938 3731 3420 0a4c 2033 3137 2e38  .998714 .L 317.8
 000010a0: 3336 3231 3720 3731 2e32 3631 3837 3220  36217 71.261872 
 000010b0: 0a4c 2033 3034 2e30 3836 3937 3420 3731  .L 304.086974 71
 000010c0: 2e32 3631 3837 3220 0a7a 0a22 2063 6c69  .261872 .z." cli
-000010d0: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-000010e0: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+000010d0: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+000010e0: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 000010f0: 3d22 6669 6c6c 3a20 2334 6261 6261 3422  ="fill: #4baba4"
 00001100: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001110: 2069 643d 2270 6174 6368 5f31 3922 3e0a   id="patch_19">.
 00001120: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001130: 3231 2e32 3733 3532 3820 3230 382e 3939  21.273528 208.99
 00001140: 3837 3134 200a 4c20 3333 352e 3032 3237  8714 .L 335.0227
 00001150: 3732 2032 3038 2e39 3938 3731 3420 0a4c  72 208.998714 .L
 00001160: 2033 3335 2e30 3232 3737 3220 3631 2e30   335.022772 61.0
 00001170: 3539 3134 3220 0a4c 2033 3231 2e32 3733  59142 .L 321.273
 00001180: 3532 3820 3631 2e30 3539 3134 3220 0a7a  528 61.059142 .z
 00001190: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000011a0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+000011a0: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 000011b0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 000011c0: 6361 6261 6422 2f3e 0a20 2020 3c2f 673e  cabad"/>.   </g>
 000011d0: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000011e0: 5f32 3022 3e0a 2020 2020 3c70 6174 6820  _20">.    <path 
 000011f0: 643d 224d 2033 3338 2e34 3630 3038 3320  d="M 338.460083 
 00001200: 3230 382e 3939 3837 3134 200a 4c20 3335  208.998714 .L 35
 00001210: 322e 3230 3933 3236 2032 3038 2e39 3938  2.209326 208.998
 00001220: 3731 3420 0a4c 2033 3532 2e32 3039 3332  714 .L 352.20932
 00001230: 3620 3335 2e35 3532 3332 200a 4c20 3333  6 35.55232 .L 33
 00001240: 382e 3436 3030 3833 2033 352e 3535 3233  8.460083 35.5523
 00001250: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001260: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
-00001270: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
+00001260: 3d22 7572 6c28 2370 3234 6234 6338 3065  ="url(#p24b4c80e
+00001270: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 00001280: 3a20 2334 6561 6262 3722 2f3e 0a20 2020  : #4eabb7"/>.   
 00001290: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 000012a0: 6174 6368 5f32 3122 3e0a 2020 2020 3c70  atch_21">.    <p
 000012b0: 6174 6820 643d 224d 2033 3535 2e36 3436  ath d="M 355.646
 000012c0: 3633 3720 3230 382e 3939 3837 3134 200a  637 208.998714 .
 000012d0: 4c20 3336 392e 3339 3538 3831 2032 3038  L 369.395881 208
 000012e0: 2e39 3938 3731 3420 0a4c 2033 3639 2e33  .998714 .L 369.3
 000012f0: 3935 3838 3120 3530 2e38 3536 3431 3320  95881 50.856413 
 00001300: 0a4c 2033 3535 2e36 3436 3633 3720 3530  .L 355.646637 50
 00001310: 2e38 3536 3431 3320 0a7a 0a22 2063 6c69  .856413 .z." cli
-00001320: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-00001330: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+00001320: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+00001330: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 00001340: 3d22 6669 6c6c 3a20 2335 3061 6363 3322  ="fill: #50acc3"
 00001350: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001360: 2069 643d 2270 6174 6368 5f32 3222 3e0a   id="patch_22">.
 00001370: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001380: 3732 2e38 3333 3139 3220 3230 382e 3939  72.833192 208.99
 00001390: 3837 3134 200a 4c20 3338 362e 3538 3234  8714 .L 386.5824
 000013a0: 3335 2032 3038 2e39 3938 3731 3420 0a4c  35 208.998714 .L
 000013b0: 2033 3836 2e35 3832 3433 3520 3435 2e37   386.582435 45.7
 000013c0: 3535 3034 3920 0a4c 2033 3732 2e38 3333  55049 .L 372.833
 000013d0: 3139 3220 3435 2e37 3535 3034 3920 0a7a  192 45.755049 .z
 000013e0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000013f0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+000013f0: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 00001400: 2073 7479 6c65 3d22 6669 6c6c 3a20 2335   style="fill: #5
 00001410: 3461 6364 3122 2f3e 0a20 2020 3c2f 673e  4acd1"/>.   </g>
 00001420: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001430: 5f32 3322 3e0a 2020 2020 3c70 6174 6820  _23">.    <path 
 00001440: 643d 224d 2033 3930 2e30 3139 3734 3620  d="M 390.019746 
 00001450: 3230 382e 3939 3837 3134 200a 4c20 3430  208.998714 .L 40
 00001460: 332e 3736 3839 3920 3230 382e 3939 3837  3.76899 208.9987
 00001470: 3134 200a 4c20 3430 332e 3736 3839 3920  14 .L 403.76899 
 00001480: 3131 322e 3037 3237 3838 200a 4c20 3339  112.072788 .L 39
 00001490: 302e 3031 3937 3436 2031 3132 2e30 3732  0.019746 112.072
 000014a0: 3738 3820 0a7a 0a22 2063 6c69 702d 7061  788 .z." clip-pa
-000014b0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-000014c0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+000014b0: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+000014c0: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 000014d0: 6c6c 3a20 2336 6461 6565 3222 2f3e 0a20  ll: #6daee2"/>. 
 000014e0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 000014f0: 2270 6174 6368 5f32 3422 3e0a 2020 2020  "patch_24">.    
 00001500: 3c70 6174 6820 643d 224d 2034 3037 2e32  <path d="M 407.2
 00001510: 3036 3330 3120 3230 382e 3939 3837 3134  06301 208.998714
 00001520: 200a 4c20 3432 302e 3935 3535 3435 2032   .L 420.955545 2
 00001530: 3038 2e39 3938 3731 3420 0a4c 2034 3230  08.998714 .L 420
 00001540: 2e39 3535 3534 3520 3132 322e 3237 3535  .955545 122.2755
 00001550: 3137 200a 4c20 3430 372e 3230 3633 3031  17 .L 407.206301
 00001560: 2031 3232 2e32 3735 3531 3720 0a7a 0a22   122.275517 .z."
 00001570: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00001580: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
+00001580: 2370 3234 6234 6338 3065 3839 2922 2073  #p24b4c80e89)" s
 00001590: 7479 6c65 3d22 6669 6c6c 3a20 2339 3461  tyle="fill: #94a
 000015a0: 6565 3822 2f3e 0a20 2020 3c2f 673e 0a20  ee8"/>.   </g>. 
 000015b0: 2020 3c67 2069 643d 2270 6174 6368 5f32    <g id="patch_2
 000015c0: 3522 3e0a 2020 2020 3c70 6174 6820 643d  5">.    <path d=
 000015d0: 224d 2034 3234 2e33 3932 3835 3520 3230  "M 424.392855 20
 000015e0: 382e 3939 3837 3134 200a 4c20 3433 382e  8.998714 .L 438.
 000015f0: 3134 3230 3939 2032 3038 2e39 3938 3731  142099 208.99871
 00001600: 3420 0a4c 2034 3338 2e31 3432 3039 3920  4 .L 438.142099 
 00001610: 3831 2e34 3634 3630 3120 0a4c 2034 3234  81.464601 .L 424
 00001620: 2e33 3932 3835 3520 3831 2e34 3634 3630  .392855 81.46460
 00001630: 3120 0a7a 0a22 2063 6c69 702d 7061 7468  1 .z." clip-path
-00001640: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
-00001650: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
+00001640: 3d22 7572 6c28 2370 3234 6234 6338 3065  ="url(#p24b4c80e
+00001650: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 00001660: 3a20 2361 6461 6265 6222 2f3e 0a20 2020  : #adabeb"/>.   
 00001670: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001680: 6174 6368 5f32 3622 3e0a 2020 2020 3c70  atch_26">.    <p
 00001690: 6174 6820 643d 224d 2034 3431 2e35 3739  ath d="M 441.579
 000016a0: 3431 2032 3038 2e39 3938 3731 3420 0a4c  41 208.998714 .L
 000016b0: 2034 3535 2e33 3238 3635 3420 3230 382e   455.328654 208.
 000016c0: 3939 3837 3134 200a 4c20 3435 352e 3332  998714 .L 455.32
 000016d0: 3836 3534 2031 3638 2e31 3837 3739 3820  8654 168.187798 
 000016e0: 0a4c 2034 3431 2e35 3739 3431 2031 3638  .L 441.57941 168
 000016f0: 2e31 3837 3739 3820 0a7a 0a22 2063 6c69  .187798 .z." cli
-00001700: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-00001710: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+00001700: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+00001710: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 00001720: 3d22 6669 6c6c 3a20 2362 6561 3465 6122  ="fill: #bea4ea"
 00001730: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001740: 2069 643d 2270 6174 6368 5f32 3722 3e0a   id="patch_27">.
 00001750: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
 00001760: 3538 2e37 3635 3936 3520 3230 382e 3939  58.765965 208.99
 00001770: 3837 3134 200a 4c20 3437 322e 3531 3532  8714 .L 472.5152
 00001780: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00001790: 2034 3732 2e35 3135 3230 3820 3135 322e   472.515208 152.
 000017a0: 3838 3337 3034 200a 4c20 3435 382e 3736  883704 .L 458.76
 000017b0: 3539 3635 2031 3532 2e38 3833 3730 3420  5965 152.883704 
 000017c0: 0a7a 0a22 2063 6c69 702d 7061 7468 3d22  .z." clip-path="
-000017d0: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
+000017d0: 7572 6c28 2370 3234 6234 6338 3065 3839  url(#p24b4c80e89
 000017e0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000017f0: 2363 6539 6265 3922 2f3e 0a20 2020 3c2f  #ce9be9"/>.   </
 00001800: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00001810: 6368 5f32 3822 3e0a 2020 2020 3c70 6174  ch_28">.    <pat
 00001820: 6820 643d 224d 2034 3735 2e39 3532 3531  h d="M 475.95251
 00001830: 3920 3230 382e 3939 3837 3134 200a 4c20  9 208.998714 .L 
 00001840: 3438 392e 3730 3137 3633 2032 3038 2e39  489.701763 208.9
 00001850: 3938 3731 3420 0a4c 2034 3839 2e37 3031  98714 .L 489.701
 00001860: 3736 3320 3134 372e 3738 3233 3420 0a4c  763 147.78234 .L
 00001870: 2034 3735 2e39 3532 3531 3920 3134 372e   475.952519 147.
 00001880: 3738 3233 3420 0a7a 0a22 2063 6c69 702d  78234 .z." clip-
-00001890: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-000018a0: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00001890: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+000018a0: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 000018b0: 6669 6c6c 3a20 2364 6638 6665 3722 2f3e  fill: #df8fe7"/>
 000018c0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 000018d0: 643d 2270 6174 6368 5f32 3922 3e0a 2020  d="patch_29">.  
 000018e0: 2020 3c70 6174 6820 643d 224d 2034 3933    <path d="M 493
 000018f0: 2e31 3339 3037 3420 3230 382e 3939 3837  .139074 208.9987
 00001900: 3134 200a 4c20 3530 362e 3838 3833 3137  14 .L 506.888317
 00001910: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001920: 3036 2e38 3838 3331 3720 3134 322e 3638  06.888317 142.68
 00001930: 3039 3735 200a 4c20 3439 332e 3133 3930  0975 .L 493.1390
 00001940: 3734 2031 3432 2e36 3830 3937 3520 0a7a  74 142.680975 .z
 00001950: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001960: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+00001960: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 00001970: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001980: 3738 6264 6222 2f3e 0a20 2020 3c2f 673e  78bdb"/>.   </g>
 00001990: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000019a0: 5f33 3022 3e0a 2020 2020 3c70 6174 6820  _30">.    <path 
 000019b0: 643d 224d 2035 3130 2e33 3235 3632 3820  d="M 510.325628 
 000019c0: 3230 382e 3939 3837 3134 200a 4c20 3532  208.998714 .L 52
 000019d0: 342e 3037 3438 3732 2032 3038 2e39 3938  4.074872 208.998
 000019e0: 3731 3420 0a4c 2035 3234 2e30 3734 3837  714 .L 524.07487
 000019f0: 3220 3133 372e 3537 3936 3131 200a 4c20  2 137.579611 .L 
 00001a00: 3531 302e 3332 3536 3238 2031 3337 2e35  510.325628 137.5
 00001a10: 3739 3631 3120 0a7a 0a22 2063 6c69 702d  79611 .z." clip-
-00001a20: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-00001a30: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00001a20: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+00001a30: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 00001a40: 6669 6c6c 3a20 2365 3838 6663 6322 2f3e  fill: #e88fcc"/>
 00001a50: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001a60: 643d 2270 6174 6368 5f33 3122 3e0a 2020  d="patch_31">.  
 00001a70: 2020 3c70 6174 6820 643d 224d 2035 3237    <path d="M 527
 00001a80: 2e35 3132 3138 3320 3230 382e 3939 3837  .512183 208.9987
 00001a90: 3134 200a 4c20 3534 312e 3236 3134 3236  14 .L 541.261426
 00001aa0: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001ab0: 3431 2e32 3631 3432 3620 3136 382e 3138  41.261426 168.18
 00001ac0: 3737 3938 200a 4c20 3532 372e 3531 3231  7798 .L 527.5121
 00001ad0: 3833 2031 3638 2e31 3837 3739 3820 0a7a  83 168.187798 .z
 00001ae0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001af0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+00001af0: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 00001b00: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001b10: 3839 3162 6622 2f3e 0a20 2020 3c2f 673e  891bf"/>.   </g>
 00001b20: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001b30: 5f33 3222 3e0a 2020 2020 3c70 6174 6820  _32">.    <path 
 00001b40: 643d 224d 2035 3434 2e36 3938 3733 3720  d="M 544.698737 
 00001b50: 3230 382e 3939 3837 3134 200a 4c20 3535  208.998714 .L 55
 00001b60: 382e 3434 3739 3831 2032 3038 2e39 3938  8.447981 208.998
 00001b70: 3731 3420 0a4c 2035 3538 2e34 3437 3938  714 .L 558.44798
 00001b80: 3120 3139 332e 3639 3436 3231 200a 4c20  1 193.694621 .L 
 00001b90: 3534 342e 3639 3837 3337 2031 3933 2e36  544.698737 193.6
 00001ba0: 3934 3632 3120 0a7a 0a22 2063 6c69 702d  94621 .z." clip-
-00001bb0: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-00001bc0: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00001bb0: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+00001bc0: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 00001bd0: 6669 6c6c 3a20 2365 3939 3462 3222 2f3e  fill: #e994b2"/>
 00001be0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001bf0: 643d 226d 6174 706c 6f74 6c69 622e 6178  d="matplotlib.ax
 00001c00: 6973 5f31 223e 0a20 2020 203c 6720 6964  is_1">.    <g id
 00001c10: 3d22 7874 6963 6b5f 3122 3e0a 2020 2020  ="xtick_1">.    
 00001c20: 203c 6720 6964 3d22 6c69 6e65 3264 5f31   <g id="line2d_1
 00001c30: 223e 0a20 2020 2020 203c 6465 6673 3e0a  ">.      <defs>.
 00001c40: 2020 2020 2020 203c 7061 7468 2069 643d         <path id=
-00001c50: 226d 6437 6633 3538 6131 3664 2220 643d  "md7f358a16d" d=
+00001c50: 226d 3733 6437 6538 3636 3562 2220 643d  "m73d7e8665b" d=
 00001c60: 224d 2030 2030 200a 4c20 3020 332e 3520  "M 0 0 .L 0 3.5 
 00001c70: 0a22 2073 7479 6c65 3d22 7374 726f 6b65  ." style="stroke
 00001c80: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00001c90: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00001ca0: 2020 2020 2020 3c2f 6465 6673 3e0a 2020        </defs>.  
 00001cb0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00001cc0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00001cd0: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
+00001cd0: 236d 3733 6437 6538 3636 3562 2220 783d  #m73d7e8665b" x=
 00001ce0: 2235 332e 3136 3332 3737 2220 793d 2232  "53.163277" y="2
 00001cf0: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 00001d00: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00001d10: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00001d20: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00001d30: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00001d40: 2020 3c67 2069 643d 2274 6578 745f 3122    <g id="text_1"
@@ -561,15 +561,15 @@
 00002300: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00002310: 2020 2020 3c2f 673e 0a20 2020 203c 2f67      </g>.    </g
 00002320: 3e0a 2020 2020 3c67 2069 643d 2278 7469  >.    <g id="xti
 00002330: 636b 5f32 223e 0a20 2020 2020 3c67 2069  ck_2">.     <g i
 00002340: 643d 226c 696e 6532 645f 3222 3e0a 2020  d="line2d_2">.  
 00002350: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00002360: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00002370: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
+00002370: 236d 3733 6437 6538 3636 3562 2220 783d  #m73d7e8665b" x=
 00002380: 2237 302e 3334 3938 3332 2220 793d 2232  "70.349832" y="2
 00002390: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 000023a0: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 000023b0: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 000023c0: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 000023d0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 000023e0: 2020 3c67 2069 643d 2274 6578 745f 3222    <g id="text_2"
@@ -628,16 +628,16 @@
 00002730: 783d 2231 3930 2e38 3639 3134 3122 2f3e  x="190.869141"/>
 00002740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00002750: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a20   </g>.    </g>. 
 00002760: 2020 203c 6720 6964 3d22 7874 6963 6b5f     <g id="xtick_
 00002770: 3322 3e0a 2020 2020 203c 6720 6964 3d22  3">.     <g id="
 00002780: 6c69 6e65 3264 5f33 223e 0a20 2020 2020  line2d_3">.     
 00002790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
-000027b0: 3766 3335 3861 3136 6422 2078 3d22 3837  7f358a16d" x="87
+000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d37   xlink:href="#m7
+000027b0: 3364 3765 3836 3635 6222 2078 3d22 3837  3d7e8665b" x="87
 000027c0: 2e35 3336 3338 3622 2079 3d22 3230 382e  .536386" y="208.
 000027d0: 3939 3837 3134 2220 7374 796c 653d 2273  998714" style="s
 000027e0: 7472 6f6b 653a 2023 3030 3030 3030 3b20  troke: #000000; 
 000027f0: 7374 726f 6b65 2d77 6964 7468 3a20 302e  stroke-width: 0.
 00002800: 3822 2f3e 0a20 2020 2020 203c 2f67 3e0a  8"/>.      </g>.
 00002810: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00002820: 6720 6964 3d22 7465 7874 5f33 223e 0a20  g id="text_3">. 
@@ -705,16 +705,16 @@
 00002c00: 2e38 3639 3134 3122 2f3e 0a20 2020 2020  .869141"/>.     
 00002c10: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00002c20: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00002c30: 6964 3d22 7874 6963 6b5f 3422 3e0a 2020  id="xtick_4">.  
 00002c40: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00002c50: 5f34 223e 0a20 2020 2020 203c 673e 0a20  _4">.      <g>. 
 00002c60: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00002c70: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
-00002c80: 3136 6422 2078 3d22 3130 342e 3732 3239  16d" x="104.7229
+00002c70: 3a68 7265 663d 2223 6d37 3364 3765 3836  :href="#m73d7e86
+00002c80: 3635 6222 2078 3d22 3130 342e 3732 3239  65b" x="104.7229
 00002c90: 3431 2220 793d 2232 3038 2e39 3938 3731  41" y="208.99871
 00002ca0: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00002cb0: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00002cc0: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00002cd0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00002ce0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00002cf0: 2274 6578 745f 3422 3e0a 2020 2020 2020  "text_4">.      
@@ -752,15 +752,15 @@
 00002ef0: 3122 2f3e 0a20 2020 2020 203c 2f67 3e0a  1"/>.      </g>.
 00002f00: 2020 2020 203c 2f67 3e0a 2020 2020 3c2f       </g>.    </
 00002f10: 673e 0a20 2020 203c 6720 6964 3d22 7874  g>.    <g id="xt
 00002f20: 6963 6b5f 3522 3e0a 2020 2020 203c 6720  ick_5">.     <g 
 00002f30: 6964 3d22 6c69 6e65 3264 5f35 223e 0a20  id="line2d_5">. 
 00002f40: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00002f50: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00002f60: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
+00002f60: 2223 6d37 3364 3765 3836 3635 6222 2078  "#m73d7e8665b" x
 00002f70: 3d22 3132 312e 3930 3934 3935 2220 793d  ="121.909495" y=
 00002f80: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00002f90: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00002fa0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00002fb0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00002fc0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00002fd0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -840,15 +840,15 @@
 00003470: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00003480: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00003490: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 000034a0: 6b5f 3622 3e0a 2020 2020 203c 6720 6964  k_6">.     <g id
 000034b0: 3d22 6c69 6e65 3264 5f36 223e 0a20 2020  ="line2d_6">.   
 000034c0: 2020 203c 673e 0a20 2020 2020 2020 3c75     <g>.       <u
 000034d0: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
-000034e0: 6d64 3766 3335 3861 3136 6422 2078 3d22  md7f358a16d" x="
+000034e0: 6d37 3364 3765 3836 3635 6222 2078 3d22  m73d7e8665b" x="
 000034f0: 3133 392e 3039 3630 3522 2079 3d22 3230  139.09605" y="20
 00003500: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003510: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003520: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003530: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003540: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003550: 203c 6720 6964 3d22 7465 7874 5f36 223e   <g id="text_6">
@@ -874,16 +874,16 @@
 00003690: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000036a0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000036b0: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 000036c0: 2069 643d 2278 7469 636b 5f37 223e 0a20   id="xtick_7">. 
 000036d0: 2020 2020 3c67 2069 643d 226c 696e 6532      <g id="line2
 000036e0: 645f 3722 3e0a 2020 2020 2020 3c67 3e0a  d_7">.      <g>.
 000036f0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00003700: 6b3a 6872 6566 3d22 236d 6437 6633 3538  k:href="#md7f358
-00003710: 6131 3664 2220 783d 2231 3536 2e32 3832  a16d" x="156.282
+00003700: 6b3a 6872 6566 3d22 236d 3733 6437 6538  k:href="#m73d7e8
+00003710: 3636 3562 2220 783d 2231 3536 2e32 3832  665b" x="156.282
 00003720: 3630 3522 2079 3d22 3230 382e 3939 3837  605" y="208.9987
 00003730: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00003740: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00003750: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00003760: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00003770: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00003780: 3d22 7465 7874 5f37 223e 0a20 2020 2020  ="text_7">.     
@@ -970,15 +970,15 @@
 00003c90: 3931 3431 222f 3e0a 2020 2020 2020 3c2f  9141"/>.      </
 00003ca0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00003cb0: 203c 2f67 3e0a 2020 2020 3c67 2069 643d   </g>.    <g id=
 00003cc0: 2278 7469 636b 5f38 223e 0a20 2020 2020  "xtick_8">.     
 00003cd0: 3c67 2069 643d 226c 696e 6532 645f 3822  <g id="line2d_8"
 00003ce0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00003cf0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00003d00: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
+00003d00: 6566 3d22 236d 3733 6437 6538 3636 3562  ef="#m73d7e8665b
 00003d10: 2220 783d 2231 3733 2e34 3639 3135 3922  " x="173.469159"
 00003d20: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00003d30: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00003d40: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00003d50: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00003d60: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00003d70: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1005,15 +1005,15 @@
 00003ec0: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00003ed0: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00003ee0: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00003ef0: 5f39 223e 0a20 2020 2020 3c67 2069 643d  _9">.     <g id=
 00003f00: 226c 696e 6532 645f 3922 3e0a 2020 2020  "line2d_9">.    
 00003f10: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00003f20: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00003f30: 6437 6633 3538 6131 3664 2220 783d 2231  d7f358a16d" x="1
+00003f30: 3733 6437 6538 3636 3562 2220 783d 2231  73d7e8665b" x="1
 00003f40: 3930 2e36 3535 3731 3422 2079 3d22 3230  90.655714" y="20
 00003f50: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003f60: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003f70: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003f80: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003f90: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003fa0: 203c 6720 6964 3d22 7465 7874 5f39 223e   <g id="text_9">
@@ -1039,16 +1039,16 @@
 000040e0: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000040f0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00004100: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00004110: 2069 643d 2278 7469 636b 5f31 3022 3e0a   id="xtick_10">.
 00004120: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00004130: 3264 5f31 3022 3e0a 2020 2020 2020 3c67  2d_10">.      <g
 00004140: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00004150: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
-00004160: 3538 6131 3664 2220 783d 2232 3037 2e38  58a16d" x="207.8
+00004150: 696e 6b3a 6872 6566 3d22 236d 3733 6437  ink:href="#m73d7
+00004160: 6538 3636 3562 2220 783d 2232 3037 2e38  e8665b" x="207.8
 00004170: 3432 3236 3822 2079 3d22 3230 382e 3939  42268" y="208.99
 00004180: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00004190: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 000041a0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 000041b0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 000041c0: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 000041d0: 6964 3d22 7465 7874 5f31 3022 3e0a 2020  id="text_10">.  
@@ -1118,16 +1118,16 @@
 000045d0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000045e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000045f0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00004600: 3d22 7874 6963 6b5f 3131 223e 0a20 2020  ="xtick_11">.   
 00004610: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00004620: 3131 223e 0a20 2020 2020 203c 673e 0a20  11">.      <g>. 
 00004630: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00004640: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
-00004650: 3136 6422 2078 3d22 3232 352e 3032 3838  16d" x="225.0288
+00004640: 3a68 7265 663d 2223 6d37 3364 3765 3836  :href="#m73d7e86
+00004650: 3635 6222 2078 3d22 3232 352e 3032 3838  65b" x="225.0288
 00004660: 3233 2220 793d 2232 3038 2e39 3938 3731  23" y="208.99871
 00004670: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00004680: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00004690: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 000046a0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000046b0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000046c0: 2274 6578 745f 3131 223e 0a20 2020 2020  "text_11">.     
@@ -1153,15 +1153,15 @@
 00004800: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00004810: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00004820: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00004830: 7469 636b 5f31 3222 3e0a 2020 2020 203c  tick_12">.     <
 00004840: 6720 6964 3d22 6c69 6e65 3264 5f31 3222  g id="line2d_12"
 00004850: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00004860: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00004870: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
+00004870: 6566 3d22 236d 3733 6437 6538 3636 3562  ef="#m73d7e8665b
 00004880: 2220 783d 2232 3432 2e32 3135 3337 3722  " x="242.215377"
 00004890: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 000048a0: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 000048b0: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 000048c0: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 000048d0: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 000048e0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1188,15 +1188,15 @@
 00004a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00004a40: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00004a50: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00004a60: 6b5f 3133 223e 0a20 2020 2020 3c67 2069  k_13">.     <g i
 00004a70: 643d 226c 696e 6532 645f 3133 223e 0a20  d="line2d_13">. 
 00004a80: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00004a90: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00004aa0: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
+00004aa0: 2223 6d37 3364 3765 3836 3635 6222 2078  "#m73d7e8665b" x
 00004ab0: 3d22 3235 392e 3430 3139 3332 2220 793d  ="259.401932" y=
 00004ac0: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00004ad0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00004ae0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00004af0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00004b00: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00004b10: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1223,15 +1223,15 @@
 00004c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00004c70: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00004c80: 2020 3c67 2069 643d 2278 7469 636b 5f31    <g id="xtick_1
 00004c90: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00004ca0: 6c69 6e65 3264 5f31 3422 3e0a 2020 2020  line2d_14">.    
 00004cb0: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00004cc0: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00004cd0: 6437 6633 3538 6131 3664 2220 783d 2232  d7f358a16d" x="2
+00004cd0: 3733 6437 6538 3636 3562 2220 783d 2232  73d7e8665b" x="2
 00004ce0: 3736 2e35 3838 3438 3622 2079 3d22 3230  76.588486" y="20
 00004cf0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00004d00: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00004d10: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00004d20: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00004d30: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00004d40: 203c 6720 6964 3d22 7465 7874 5f31 3422   <g id="text_14"
@@ -1257,16 +1257,16 @@
 00004e80: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00004e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00004ea0: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00004eb0: 6720 6964 3d22 7874 6963 6b5f 3135 223e  g id="xtick_15">
 00004ec0: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00004ed0: 6532 645f 3135 223e 0a20 2020 2020 203c  e2d_15">.      <
 00004ee0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d64 3766  link:href="#md7f
-00004f00: 3335 3861 3136 6422 2078 3d22 3239 332e  358a16d" x="293.
+00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d37 3364  link:href="#m73d
+00004f00: 3765 3836 3635 6222 2078 3d22 3239 332e  7e8665b" x="293.
 00004f10: 3737 3530 3431 2220 793d 2232 3038 2e39  775041" y="208.9
 00004f20: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 00004f30: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00004f40: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00004f50: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00004f60: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00004f70: 2069 643d 2274 6578 745f 3135 223e 0a20   id="text_15">. 
@@ -1292,16 +1292,16 @@
 000050b0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000050c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000050d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000050e0: 3d22 7874 6963 6b5f 3136 223e 0a20 2020  ="xtick_16">.   
 000050f0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005100: 3136 223e 0a20 2020 2020 203c 673e 0a20  16">.      <g>. 
 00005110: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005120: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
-00005130: 3136 6422 2078 3d22 3331 302e 3936 3135  16d" x="310.9615
+00005120: 3a68 7265 663d 2223 6d37 3364 3765 3836  :href="#m73d7e86
+00005130: 3635 6222 2078 3d22 3331 302e 3936 3135  65b" x="310.9615
 00005140: 3935 2220 793d 2232 3038 2e39 3938 3731  95" y="208.99871
 00005150: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005160: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005170: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005180: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005190: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000051a0: 2274 6578 745f 3136 223e 0a20 2020 2020  "text_16">.     
@@ -1327,15 +1327,15 @@
 000052e0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000052f0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005300: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005310: 7469 636b 5f31 3722 3e0a 2020 2020 203c  tick_17">.     <
 00005320: 6720 6964 3d22 6c69 6e65 3264 5f31 3722  g id="line2d_17"
 00005330: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005340: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005350: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
+00005350: 6566 3d22 236d 3733 6437 6538 3636 3562  ef="#m73d7e8665b
 00005360: 2220 783d 2233 3238 2e31 3438 3135 2220  " x="328.14815" 
 00005370: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00005380: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 00005390: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000053a0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000053b0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000053c0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
@@ -1362,15 +1362,15 @@
 00005510: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00005520: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00005530: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00005540: 5f31 3822 3e0a 2020 2020 203c 6720 6964  _18">.     <g id
 00005550: 3d22 6c69 6e65 3264 5f31 3822 3e0a 2020  ="line2d_18">.  
 00005560: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00005570: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00005580: 236d 6437 6633 3538 6131 3664 2220 783d  #md7f358a16d" x=
+00005580: 236d 3733 6437 6538 3636 3562 2220 783d  #m73d7e8665b" x=
 00005590: 2233 3435 2e33 3334 3730 3522 2079 3d22  "345.334705" y="
 000055a0: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 000055b0: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 000055c0: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 000055d0: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 000055e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000055f0: 2020 203c 6720 6964 3d22 7465 7874 5f31     <g id="text_1
@@ -1396,16 +1396,16 @@
 00005730: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00005740: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00005750: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00005760: 203c 6720 6964 3d22 7874 6963 6b5f 3139   <g id="xtick_19
 00005770: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00005780: 696e 6532 645f 3139 223e 0a20 2020 2020  ine2d_19">.     
 00005790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
-000057b0: 3766 3335 3861 3136 6422 2078 3d22 3336  7f358a16d" x="36
+000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d37   xlink:href="#m7
+000057b0: 3364 3765 3836 3635 6222 2078 3d22 3336  3d7e8665b" x="36
 000057c0: 322e 3532 3132 3539 2220 793d 2232 3038  2.521259" y="208
 000057d0: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 000057e0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 000057f0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00005800: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00005810: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00005820: 3c67 2069 643d 2274 6578 745f 3139 223e  <g id="text_19">
@@ -1431,16 +1431,16 @@
 00005960: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00005970: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00005980: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00005990: 2069 643d 2278 7469 636b 5f32 3022 3e0a   id="xtick_20">.
 000059a0: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 000059b0: 3264 5f32 3022 3e0a 2020 2020 2020 3c67  2d_20">.      <g
 000059c0: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-000059d0: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
-000059e0: 3538 6131 3664 2220 783d 2233 3739 2e37  58a16d" x="379.7
+000059d0: 696e 6b3a 6872 6566 3d22 236d 3733 6437  ink:href="#m73d7
+000059e0: 6538 3636 3562 2220 783d 2233 3739 2e37  e8665b" x="379.7
 000059f0: 3037 3831 3422 2079 3d22 3230 382e 3939  07814" y="208.99
 00005a00: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00005a10: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00005a20: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00005a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00005a40: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00005a50: 6964 3d22 7465 7874 5f32 3022 3e0a 2020  id="text_20">.  
@@ -1466,16 +1466,16 @@
 00005b90: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 00005ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00005bb0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00005bc0: 3d22 7874 6963 6b5f 3231 223e 0a20 2020  ="xtick_21">.   
 00005bd0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005be0: 3231 223e 0a20 2020 2020 203c 673e 0a20  21">.      <g>. 
 00005bf0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005c00: 3a68 7265 663d 2223 6d64 3766 3335 3861  :href="#md7f358a
-00005c10: 3136 6422 2078 3d22 3339 362e 3839 3433  16d" x="396.8943
+00005c00: 3a68 7265 663d 2223 6d37 3364 3765 3836  :href="#m73d7e86
+00005c10: 3635 6222 2078 3d22 3339 362e 3839 3433  65b" x="396.8943
 00005c20: 3638 2220 793d 2232 3038 2e39 3938 3731  68" y="208.99871
 00005c30: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005c40: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005c50: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005c70: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00005c80: 2274 6578 745f 3231 223e 0a20 2020 2020  "text_21">.     
@@ -1501,15 +1501,15 @@
 00005dc0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00005dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005de0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005df0: 7469 636b 5f32 3222 3e0a 2020 2020 203c  tick_22">.     <
 00005e00: 6720 6964 3d22 6c69 6e65 3264 5f32 3222  g id="line2d_22"
 00005e10: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005e20: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005e30: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
+00005e30: 6566 3d22 236d 3733 6437 6538 3636 3562  ef="#m73d7e8665b
 00005e40: 2220 783d 2234 3134 2e30 3830 3932 3322  " x="414.080923"
 00005e50: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00005e60: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00005e70: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00005e80: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00005e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00005ea0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1536,15 +1536,15 @@
 00005ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006000: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006010: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006020: 6b5f 3233 223e 0a20 2020 2020 3c67 2069  k_23">.     <g i
 00006030: 643d 226c 696e 6532 645f 3233 223e 0a20  d="line2d_23">. 
 00006040: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006050: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006060: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
+00006060: 2223 6d37 3364 3765 3836 3635 6222 2078  "#m73d7e8665b" x
 00006070: 3d22 3433 312e 3236 3734 3737 2220 793d  ="431.267477" y=
 00006080: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00006090: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 000060a0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 000060b0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 000060c0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 000060d0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1571,15 +1571,15 @@
 00006220: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00006230: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00006240: 2020 3c67 2069 643d 2278 7469 636b 5f32    <g id="xtick_2
 00006250: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00006260: 6c69 6e65 3264 5f32 3422 3e0a 2020 2020  line2d_24">.    
 00006270: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00006280: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00006290: 6437 6633 3538 6131 3664 2220 783d 2234  d7f358a16d" x="4
+00006290: 3733 6437 6538 3636 3562 2220 783d 2234  73d7e8665b" x="4
 000062a0: 3438 2e34 3534 3033 3222 2079 3d22 3230  48.454032" y="20
 000062b0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 000062c0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000062d0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000062e0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000062f0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00006300: 203c 6720 6964 3d22 7465 7874 5f32 3422   <g id="text_24"
@@ -1605,16 +1605,16 @@
 00006440: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00006450: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006460: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00006470: 6720 6964 3d22 7874 6963 6b5f 3235 223e  g id="xtick_25">
 00006480: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00006490: 6532 645f 3235 223e 0a20 2020 2020 203c  e2d_25">.      <
 000064a0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d64 3766  link:href="#md7f
-000064c0: 3335 3861 3136 6422 2078 3d22 3436 352e  358a16d" x="465.
+000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d37 3364  link:href="#m73d
+000064c0: 3765 3836 3635 6222 2078 3d22 3436 352e  7e8665b" x="465.
 000064d0: 3634 3035 3836 2220 793d 2232 3038 2e39  640586" y="208.9
 000064e0: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 000064f0: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00006500: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00006510: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00006520: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00006530: 2069 643d 2274 6578 745f 3235 223e 0a20   id="text_25">. 
@@ -1640,16 +1640,16 @@
 00006670: 3836 3931 3431 222f 3e0a 2020 2020 2020  869141"/>.      
 00006680: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00006690: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 000066a0: 643d 2278 7469 636b 5f32 3622 3e0a 2020  d="xtick_26">.  
 000066b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000066c0: 5f32 3622 3e0a 2020 2020 2020 3c67 3e0a  _26">.      <g>.
 000066d0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-000066e0: 6b3a 6872 6566 3d22 236d 6437 6633 3538  k:href="#md7f358
-000066f0: 6131 3664 2220 783d 2234 3832 2e38 3237  a16d" x="482.827
+000066e0: 6b3a 6872 6566 3d22 236d 3733 6437 6538  k:href="#m73d7e8
+000066f0: 3636 3562 2220 783d 2234 3832 2e38 3237  665b" x="482.827
 00006700: 3134 3122 2079 3d22 3230 382e 3939 3837  141" y="208.9987
 00006710: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00006720: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00006730: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00006740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00006750: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00006760: 3d22 7465 7874 5f32 3622 3e0a 2020 2020  ="text_26">.    
@@ -1675,15 +1675,15 @@
 000068a0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000068b0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 000068c0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 000068d0: 7469 636b 5f32 3722 3e0a 2020 2020 203c  tick_27">.     <
 000068e0: 6720 6964 3d22 6c69 6e65 3264 5f32 3722  g id="line2d_27"
 000068f0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00006900: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00006910: 6566 3d22 236d 6437 6633 3538 6131 3664  ef="#md7f358a16d
+00006910: 6566 3d22 236d 3733 6437 6538 3636 3562  ef="#m73d7e8665b
 00006920: 2220 783d 2235 3030 2e30 3133 3639 3522  " x="500.013695"
 00006930: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00006940: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00006950: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00006960: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00006970: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006980: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1710,15 +1710,15 @@
 00006ad0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006ae0: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006af0: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006b00: 6b5f 3238 223e 0a20 2020 2020 3c67 2069  k_28">.     <g i
 00006b10: 643d 226c 696e 6532 645f 3238 223e 0a20  d="line2d_28">. 
 00006b20: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006b30: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006b40: 2223 6d64 3766 3335 3861 3136 6422 2078  "#md7f358a16d" x
+00006b40: 2223 6d37 3364 3765 3836 3635 6222 2078  "#m73d7e8665b" x
 00006b50: 3d22 3531 372e 3230 3032 3522 2079 3d22  ="517.20025" y="
 00006b60: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 00006b70: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00006b80: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00006b90: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00006ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00006bb0: 2020 203c 6720 6964 3d22 7465 7874 5f32     <g id="text_2
@@ -1744,16 +1744,16 @@
 00006cf0: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00006d00: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00006d10: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00006d20: 203c 6720 6964 3d22 7874 6963 6b5f 3239   <g id="xtick_29
 00006d30: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00006d40: 696e 6532 645f 3239 223e 0a20 2020 2020  ine2d_29">.     
 00006d50: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d64   xlink:href="#md
-00006d70: 3766 3335 3861 3136 6422 2078 3d22 3533  7f358a16d" x="53
+00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d37   xlink:href="#m7
+00006d70: 3364 3765 3836 3635 6222 2078 3d22 3533  3d7e8665b" x="53
 00006d80: 342e 3338 3638 3035 2220 793d 2232 3038  4.386805" y="208
 00006d90: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 00006da0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 00006db0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00006dc0: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00006dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00006de0: 3c67 2069 643d 2274 6578 745f 3239 223e  <g id="text_29">
@@ -1779,16 +1779,16 @@
 00006f20: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00006f30: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00006f40: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00006f50: 2069 643d 2278 7469 636b 5f33 3022 3e0a   id="xtick_30">.
 00006f60: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00006f70: 3264 5f33 3022 3e0a 2020 2020 2020 3c67  2d_30">.      <g
 00006f80: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00006f90: 696e 6b3a 6872 6566 3d22 236d 6437 6633  ink:href="#md7f3
-00006fa0: 3538 6131 3664 2220 783d 2235 3531 2e35  58a16d" x="551.5
+00006f90: 696e 6b3a 6872 6566 3d22 236d 3733 6437  ink:href="#m73d7
+00006fa0: 6538 3636 3562 2220 783d 2235 3531 2e35  e8665b" x="551.5
 00006fb0: 3733 3335 3922 2079 3d22 3230 382e 3939  73359" y="208.99
 00006fc0: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00006fd0: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00006fe0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00006ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007000: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00007010: 6964 3d22 7465 7874 5f33 3022 3e0a 2020  id="text_30">.  
@@ -1816,24 +1816,24 @@
 00007170: 2020 3c2f 673e 0a20 2020 3c2f 673e 0a20    </g>.   </g>. 
 00007180: 2020 3c67 2069 643d 226d 6174 706c 6f74    <g id="matplot
 00007190: 6c69 622e 6178 6973 5f32 223e 0a20 2020  lib.axis_2">.   
 000071a0: 203c 6720 6964 3d22 7974 6963 6b5f 3122   <g id="ytick_1"
 000071b0: 3e0a 2020 2020 203c 6720 6964 3d22 6c69  >.     <g id="li
 000071c0: 6e65 3264 5f33 3122 3e0a 2020 2020 2020  ne2d_31">.      
 000071d0: 3c64 6566 733e 0a20 2020 2020 2020 3c70  <defs>.       <p
-000071e0: 6174 6820 6964 3d22 6d30 3034 6533 3533  ath id="m004e353
-000071f0: 3338 3922 2064 3d22 4d20 3020 3020 0a4c  389" d="M 0 0 .L
+000071e0: 6174 6820 6964 3d22 6d38 6337 3437 3136  ath id="m8c74716
+000071f0: 3438 6222 2064 3d22 4d20 3020 3020 0a4c  48b" d="M 0 0 .L
 00007200: 202d 332e 3520 3020 0a22 2073 7479 6c65   -3.5 0 ." style
 00007210: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00007220: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00007230: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00007240: 6465 6673 3e0a 2020 2020 2020 3c67 3e0a  defs>.      <g>.
 00007250: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007260: 6b3a 6872 6566 3d22 236d 3030 3465 3335  k:href="#m004e35
-00007270: 3333 3839 2220 783d 2234 342e 3537 2220  3389" x="44.57" 
+00007260: 6b3a 6872 6566 3d22 236d 3863 3734 3731  k:href="#m8c7471
+00007270: 3634 3862 2220 783d 2234 342e 3537 2220  648b" x="44.57" 
 00007280: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00007290: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 000072a0: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000072b0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000072c0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000072d0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
 000072e0: 745f 3331 223e 0a20 2020 2020 203c 212d  t_31">.      <!-
@@ -1847,15 +1847,15 @@
 00007360: 3330 222f 3e0a 2020 2020 2020 3c2f 673e  30"/>.      </g>
 00007370: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007380: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007390: 7469 636b 5f32 223e 0a20 2020 2020 3c67  tick_2">.     <g
 000073a0: 2069 643d 226c 696e 6532 645f 3332 223e   id="line2d_32">
 000073b0: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 000073c0: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-000073d0: 663d 2223 6d30 3034 6533 3533 3338 3922  f="#m004e353389"
+000073d0: 663d 2223 6d38 6337 3437 3136 3438 6222  f="#m8c7471648b"
 000073e0: 2078 3d22 3434 2e35 3722 2079 3d22 3138   x="44.57" y="18
 000073f0: 332e 3439 3138 3932 2220 7374 796c 653d  3.491892" style=
 00007400: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00007410: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00007420: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00007430: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00007440: 203c 6720 6964 3d22 7465 7874 5f33 3222   <g id="text_32"
@@ -1869,16 +1869,16 @@
 000074c0: 656a 6156 7553 616e 732d 3335 222f 3e0a  ejaVuSans-35"/>.
 000074d0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000074e0: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 000074f0: 2020 3c67 2069 643d 2279 7469 636b 5f33    <g id="ytick_3
 00007500: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00007510: 696e 6532 645f 3333 223e 0a20 2020 2020  ine2d_33">.     
 00007520: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d30   xlink:href="#m0
-00007540: 3034 6533 3533 3338 3922 2078 3d22 3434  04e353389" x="44
+00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d38   xlink:href="#m8
+00007540: 6337 3437 3136 3438 6222 2078 3d22 3434  c7471648b" x="44
 00007550: 2e35 3722 2079 3d22 3135 372e 3938 3530  .57" y="157.9850
 00007560: 3639 2220 7374 796c 653d 2273 7472 6f6b  69" style="strok
 00007570: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00007580: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00007590: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 000075a0: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 000075b0: 3d22 7465 7874 5f33 3322 3e0a 2020 2020  ="text_33">.    
@@ -1896,15 +1896,15 @@
 00007670: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007680: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00007690: 0a20 2020 203c 6720 6964 3d22 7974 6963  .    <g id="ytic
 000076a0: 6b5f 3422 3e0a 2020 2020 203c 6720 6964  k_4">.     <g id
 000076b0: 3d22 6c69 6e65 3264 5f33 3422 3e0a 2020  ="line2d_34">.  
 000076c0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 000076d0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-000076e0: 236d 3030 3465 3335 3333 3839 2220 783d  #m004e353389" x=
+000076e0: 236d 3863 3734 3731 3634 3862 2220 783d  #m8c7471648b" x=
 000076f0: 2234 342e 3537 2220 793d 2231 3332 2e34  "44.57" y="132.4
 00007700: 3738 3234 3622 2073 7479 6c65 3d22 7374  78246" style="st
 00007710: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00007720: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00007730: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00007740: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00007750: 2069 643d 2274 6578 745f 3334 223e 0a20   id="text_34">. 
@@ -1922,15 +1922,15 @@
 00007810: 3437 222f 3e0a 2020 2020 2020 3c2f 673e  47"/>.      </g>
 00007820: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007830: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007840: 7469 636b 5f35 223e 0a20 2020 2020 3c67  tick_5">.     <g
 00007850: 2069 643d 226c 696e 6532 645f 3335 223e   id="line2d_35">
 00007860: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 00007870: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-00007880: 663d 2223 6d30 3034 6533 3533 3338 3922  f="#m004e353389"
+00007880: 663d 2223 6d38 6337 3437 3136 3438 6222  f="#m8c7471648b"
 00007890: 2078 3d22 3434 2e35 3722 2079 3d22 3130   x="44.57" y="10
 000078a0: 362e 3937 3134 3233 2220 7374 796c 653d  6.971423" style=
 000078b0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000078c0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000078d0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000078e0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 000078f0: 203c 6720 6964 3d22 7465 7874 5f33 3522   <g id="text_35"
@@ -1948,16 +1948,16 @@
 000079b0: 3233 3034 3722 2f3e 0a20 2020 2020 203c  23047"/>.      <
 000079c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000079d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000079e0: 3d22 7974 6963 6b5f 3622 3e0a 2020 2020  ="ytick_6">.    
 000079f0: 203c 6720 6964 3d22 6c69 6e65 3264 5f33   <g id="line2d_3
 00007a00: 3622 3e0a 2020 2020 2020 3c67 3e0a 2020  6">.      <g>.  
 00007a10: 2020 2020 203c 7573 6520 786c 696e 6b3a       <use xlink:
-00007a20: 6872 6566 3d22 236d 3030 3465 3335 3333  href="#m004e3533
-00007a30: 3839 2220 783d 2234 342e 3537 2220 793d  89" x="44.57" y=
+00007a20: 6872 6566 3d22 236d 3863 3734 3731 3634  href="#m8c747164
+00007a30: 3862 2220 783d 2234 342e 3537 2220 793d  8b" x="44.57" y=
 00007a40: 2238 312e 3436 3436 3031 2220 7374 796c  "81.464601" styl
 00007a50: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00007a60: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00007a70: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00007a80: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00007a90: 2020 203c 6720 6964 3d22 7465 7874 5f33     <g id="text_3
 00007aa0: 3622 3e0a 2020 2020 2020 3c21 2d2d 2032  6">.      <!-- 2
@@ -1974,16 +1974,16 @@
 00007b50: 3632 3330 3437 222f 3e0a 2020 2020 2020  623047"/>.      
 00007b60: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007b70: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 00007b80: 643d 2279 7469 636b 5f37 223e 0a20 2020  d="ytick_7">.   
 00007b90: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00007ba0: 3337 223e 0a20 2020 2020 203c 673e 0a20  37">.      <g>. 
 00007bb0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00007bc0: 3a68 7265 663d 2223 6d30 3034 6533 3533  :href="#m004e353
-00007bd0: 3338 3922 2078 3d22 3434 2e35 3722 2079  389" x="44.57" y
+00007bc0: 3a68 7265 663d 2223 6d38 6337 3437 3136  :href="#m8c74716
+00007bd0: 3438 6222 2078 3d22 3434 2e35 3722 2079  48b" x="44.57" y
 00007be0: 3d22 3535 2e39 3537 3737 3822 2073 7479  ="55.957778" sty
 00007bf0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00007c00: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00007c10: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00007c20: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007c30: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
 00007c40: 3337 223e 0a20 2020 2020 203c 212d 2d20  37">.      <!-- 
@@ -2000,16 +2000,16 @@
 00007cf0: 2e36 3233 3034 3722 2f3e 0a20 2020 2020  .623047"/>.     
 00007d00: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007d10: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00007d20: 6964 3d22 7974 6963 6b5f 3822 3e0a 2020  id="ytick_8">.  
 00007d30: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00007d40: 5f33 3822 3e0a 2020 2020 2020 3c67 3e0a  _38">.      <g>.
 00007d50: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007d60: 6b3a 6872 6566 3d22 236d 3030 3465 3335  k:href="#m004e35
-00007d70: 3333 3839 2220 783d 2234 342e 3537 2220  3389" x="44.57" 
+00007d60: 6b3a 6872 6566 3d22 236d 3863 3734 3731  k:href="#m8c7471
+00007d70: 3634 3862 2220 783d 2234 342e 3537 2220  648b" x="44.57" 
 00007d80: 793d 2233 302e 3435 3039 3535 2220 7374  y="30.450955" st
 00007d90: 796c 653d 2273 7472 6f6b 653a 2023 3030  yle="stroke: #00
 00007da0: 3030 3030 3b20 7374 726f 6b65 2d77 6964  0000; stroke-wid
 00007db0: 7468 3a20 302e 3822 2f3e 0a20 2020 2020  th: 0.8"/>.     
 00007dc0: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007dd0: 2020 2020 203c 6720 6964 3d22 7465 7874       <g id="text
 00007de0: 5f33 3822 3e0a 2020 2020 2020 3c21 2d2d  _38">.      <!--
@@ -2354,289 +2354,289 @@
 00009310: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
 00009320: 616e 732d 3733 2220 783d 2235 3438 2e37  ans-73" x="548.7
 00009330: 3837 3130 3922 2f3e 0a20 2020 2020 3c2f  87109"/>.     </
 00009340: 673e 0a20 2020 203c 2f67 3e0a 2020 203c  g>.    </g>.   <
 00009350: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009360: 6e65 3264 5f33 3922 3e0a 2020 2020 3c70  ne2d_39">.    <p
 00009370: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009380: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
+00009380: 726c 2823 7032 3462 3463 3830 6538 3929  rl(#p24b4c80e89)
 00009390: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 000093a0: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 000093b0: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 000093c0: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 000093d0: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 000093e0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 000093f0: 2069 643d 226c 696e 6532 645f 3430 223e   id="line2d_40">
 00009400: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009410: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-00009420: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00009410: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+00009420: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 00009430: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009440: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009450: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009460: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009470: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009480: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009490: 3264 5f34 3122 3e0a 2020 2020 3c70 6174  2d_41">.    <pat
 000094a0: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-000094b0: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
+000094b0: 2823 7032 3462 3463 3830 6538 3929 2220  (#p24b4c80e89)" 
 000094c0: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 000094d0: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 000094e0: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 000094f0: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009500: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009510: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009520: 643d 226c 696e 6532 645f 3432 223e 0a20  d="line2d_42">. 
 00009530: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009540: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-00009550: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+00009540: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+00009550: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 00009560: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009570: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009580: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009590: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 000095a0: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 000095b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000095c0: 5f34 3322 3e0a 2020 2020 3c70 6174 6820  _43">.    <path 
 000095d0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-000095e0: 7032 3261 3136 6136 6462 6429 2220 7374  p22a16a6dbd)" st
+000095e0: 7032 3462 3463 3830 6538 3929 2220 7374  p24b4c80e89)" st
 000095f0: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009600: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009610: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009620: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009630: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009640: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009650: 226c 696e 6532 645f 3434 223e 0a20 2020  "line2d_44">.   
 00009660: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009670: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
-00009680: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
+00009670: 3d22 7572 6c28 2370 3234 6234 6338 3065  ="url(#p24b4c80e
+00009680: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 00009690: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 000096a0: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 000096b0: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 000096c0: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 000096d0: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 000096e0: 203c 6720 6964 3d22 6c69 6e65 3264 5f34   <g id="line2d_4
 000096f0: 3522 3e0a 2020 2020 3c70 6174 6820 636c  5">.    <path cl
 00009700: 6970 2d70 6174 683d 2275 726c 2823 7032  ip-path="url(#p2
-00009710: 3261 3136 6136 6462 6429 2220 7374 796c  2a16a6dbd)" styl
+00009710: 3462 3463 3830 6538 3929 2220 7374 796c  4b4c80e89)" styl
 00009720: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 00009730: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 00009740: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 00009750: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 00009760: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 00009770: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 00009780: 696e 6532 645f 3436 223e 0a20 2020 203c  ine2d_46">.    <
 00009790: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-000097a0: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
+000097a0: 7572 6c28 2370 3234 6234 6338 3065 3839  url(#p24b4c80e89
 000097b0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000097c0: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 000097d0: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 000097e0: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 000097f0: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 00009800: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00009810: 6720 6964 3d22 6c69 6e65 3264 5f34 3722  g id="line2d_47"
 00009820: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-00009830: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
-00009840: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
+00009830: 2d70 6174 683d 2275 726c 2823 7032 3462  -path="url(#p24b
+00009840: 3463 3830 6538 3929 2220 7374 796c 653d  4c80e89)" style=
 00009850: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 00009860: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 00009870: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 00009880: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 00009890: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 000098a0: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 000098b0: 6532 645f 3438 223e 0a20 2020 203c 7061  e2d_48">.    <pa
 000098c0: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-000098d0: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+000098d0: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 000098e0: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 000098f0: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 00009900: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 00009910: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 00009920: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 00009930: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00009940: 6964 3d22 6c69 6e65 3264 5f34 3922 3e0a  id="line2d_49">.
 00009950: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-00009960: 6174 683d 2275 726c 2823 7032 3261 3136  ath="url(#p22a16
-00009970: 6136 6462 6429 2220 7374 796c 653d 2266  a6dbd)" style="f
+00009960: 6174 683d 2275 726c 2823 7032 3462 3463  ath="url(#p24b4c
+00009970: 3830 6538 3929 2220 7374 796c 653d 2266  80e89)" style="f
 00009980: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 00009990: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 000099a0: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 000099b0: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 000099c0: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 000099d0: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 000099e0: 645f 3530 223e 0a20 2020 203c 7061 7468  d_50">.    <path
 000099f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00009a00: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
+00009a00: 2370 3234 6234 6338 3065 3839 2922 2073  #p24b4c80e89)" s
 00009a10: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 00009a20: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 00009a30: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 00009a40: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 00009a50: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 00009a60: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 00009a70: 3d22 6c69 6e65 3264 5f35 3122 3e0a 2020  ="line2d_51">.  
 00009a80: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-00009a90: 683d 2275 726c 2823 7032 3261 3136 6136  h="url(#p22a16a6
-00009aa0: 6462 6429 2220 7374 796c 653d 2266 696c  dbd)" style="fil
+00009a90: 683d 2275 726c 2823 7032 3462 3463 3830  h="url(#p24b4c80
+00009aa0: 6538 3929 2220 7374 796c 653d 2266 696c  e89)" style="fil
 00009ab0: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 00009ac0: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 00009ad0: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 00009ae0: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 00009af0: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 00009b00: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00009b10: 3532 223e 0a20 2020 203c 7061 7468 2063  52">.    <path c
 00009b20: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00009b30: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
+00009b30: 3234 6234 6338 3065 3839 2922 2073 7479  24b4c80e89)" sty
 00009b40: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 00009b50: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 00009b60: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 00009b70: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 00009b80: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 00009b90: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 00009ba0: 6c69 6e65 3264 5f35 3322 3e0a 2020 2020  line2d_53">.    
 00009bb0: 3c70 6174 6820 636c 6970 2d70 6174 683d  <path clip-path=
-00009bc0: 2275 726c 2823 7032 3261 3136 6136 6462  "url(#p22a16a6db
-00009bd0: 6429 2220 7374 796c 653d 2266 696c 6c3a  d)" style="fill:
+00009bc0: 2275 726c 2823 7032 3462 3463 3830 6538  "url(#p24b4c80e8
+00009bd0: 3929 2220 7374 796c 653d 2266 696c 6c3a  9)" style="fill:
 00009be0: 206e 6f6e 653b 2073 7472 6f6b 653a 2023   none; stroke: #
 00009bf0: 3432 3432 3432 3b20 7374 726f 6b65 2d77  424242; stroke-w
 00009c00: 6964 7468 3a20 322e 373b 2073 7472 6f6b  idth: 2.7; strok
 00009c10: 652d 6c69 6e65 6361 703a 2073 7175 6172  e-linecap: squar
 00009c20: 6522 2f3e 0a20 2020 3c2f 673e 0a20 2020  e"/>.   </g>.   
 00009c30: 3c67 2069 643d 226c 696e 6532 645f 3534  <g id="line2d_54
 00009c40: 223e 0a20 2020 203c 7061 7468 2063 6c69  ">.    <path cli
-00009c50: 702d 7061 7468 3d22 7572 6c28 2370 3232  p-path="url(#p22
-00009c60: 6131 3661 3664 6264 2922 2073 7479 6c65  a16a6dbd)" style
+00009c50: 702d 7061 7468 3d22 7572 6c28 2370 3234  p-path="url(#p24
+00009c60: 6234 6338 3065 3839 2922 2073 7479 6c65  b4c80e89)" style
 00009c70: 3d22 6669 6c6c 3a20 6e6f 6e65 3b20 7374  ="fill: none; st
 00009c80: 726f 6b65 3a20 2334 3234 3234 323b 2073  roke: #424242; s
 00009c90: 7472 6f6b 652d 7769 6474 683a 2032 2e37  troke-width: 2.7
 00009ca0: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00009cb0: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00009cc0: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009cd0: 6e65 3264 5f35 3522 3e0a 2020 2020 3c70  ne2d_55">.    <p
 00009ce0: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009cf0: 726c 2823 7032 3261 3136 6136 6462 6429  rl(#p22a16a6dbd)
+00009cf0: 726c 2823 7032 3462 3463 3830 6538 3929  rl(#p24b4c80e89)
 00009d00: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 00009d10: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 00009d20: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 00009d30: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 00009d40: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 00009d50: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00009d60: 2069 643d 226c 696e 6532 645f 3536 223e   id="line2d_56">
 00009d70: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009d80: 7061 7468 3d22 7572 6c28 2370 3232 6131  path="url(#p22a1
-00009d90: 3661 3664 6264 2922 2073 7479 6c65 3d22  6a6dbd)" style="
+00009d80: 7061 7468 3d22 7572 6c28 2370 3234 6234  path="url(#p24b4
+00009d90: 6338 3065 3839 2922 2073 7479 6c65 3d22  c80e89)" style="
 00009da0: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009db0: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009dc0: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009dd0: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009de0: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009df0: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009e00: 3264 5f35 3722 3e0a 2020 2020 3c70 6174  2d_57">.    <pat
 00009e10: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-00009e20: 2823 7032 3261 3136 6136 6462 6429 2220  (#p22a16a6dbd)" 
+00009e20: 2823 7032 3462 3463 3830 6538 3929 2220  (#p24b4c80e89)" 
 00009e30: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 00009e40: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 00009e50: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 00009e60: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009e70: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009e80: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009e90: 643d 226c 696e 6532 645f 3538 223e 0a20  d="line2d_58">. 
 00009ea0: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009eb0: 7468 3d22 7572 6c28 2370 3232 6131 3661  th="url(#p22a16a
-00009ec0: 3664 6264 2922 2073 7479 6c65 3d22 6669  6dbd)" style="fi
+00009eb0: 7468 3d22 7572 6c28 2370 3234 6234 6338  th="url(#p24b4c8
+00009ec0: 3065 3839 2922 2073 7479 6c65 3d22 6669  0e89)" style="fi
 00009ed0: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009ee0: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009ef0: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009f00: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 00009f10: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 00009f20: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00009f30: 5f35 3922 3e0a 2020 2020 3c70 6174 6820  _59">.    <path 
 00009f40: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00009f50: 7032 3261 3136 6136 6462 6429 2220 7374  p22a16a6dbd)" st
+00009f50: 7032 3462 3463 3830 6538 3929 2220 7374  p24b4c80e89)" st
 00009f60: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009f70: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009f80: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009f90: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009fa0: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009fb0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009fc0: 226c 696e 6532 645f 3630 223e 0a20 2020  "line2d_60">.   
 00009fd0: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009fe0: 3d22 7572 6c28 2370 3232 6131 3661 3664  ="url(#p22a16a6d
-00009ff0: 6264 2922 2073 7479 6c65 3d22 6669 6c6c  bd)" style="fill
+00009fe0: 3d22 7572 6c28 2370 3234 6234 6338 3065  ="url(#p24b4c80e
+00009ff0: 3839 2922 2073 7479 6c65 3d22 6669 6c6c  89)" style="fill
 0000a000: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 0000a010: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 0000a020: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 0000a030: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 0000a040: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 0000a050: 203c 6720 6964 3d22 6c69 6e65 3264 5f36   <g id="line2d_6
 0000a060: 3122 3e0a 2020 2020 3c70 6174 6820 636c  1">.    <path cl
 0000a070: 6970 2d70 6174 683d 2275 726c 2823 7032  ip-path="url(#p2
-0000a080: 3261 3136 6136 6462 6429 2220 7374 796c  2a16a6dbd)" styl
+0000a080: 3462 3463 3830 6538 3929 2220 7374 796c  4b4c80e89)" styl
 0000a090: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 0000a0a0: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 0000a0b0: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 0000a0c0: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 0000a0d0: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 0000a0e0: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 0000a0f0: 696e 6532 645f 3632 223e 0a20 2020 203c  ine2d_62">.    <
 0000a100: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-0000a110: 7572 6c28 2370 3232 6131 3661 3664 6264  url(#p22a16a6dbd
+0000a110: 7572 6c28 2370 3234 6234 6338 3065 3839  url(#p24b4c80e89
 0000a120: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 0000a130: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 0000a140: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 0000a150: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 0000a160: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 0000a170: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 0000a180: 6720 6964 3d22 6c69 6e65 3264 5f36 3322  g id="line2d_63"
 0000a190: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-0000a1a0: 2d70 6174 683d 2275 726c 2823 7032 3261  -path="url(#p22a
-0000a1b0: 3136 6136 6462 6429 2220 7374 796c 653d  16a6dbd)" style=
+0000a1a0: 2d70 6174 683d 2275 726c 2823 7032 3462  -path="url(#p24b
+0000a1b0: 3463 3830 6538 3929 2220 7374 796c 653d  4c80e89)" style=
 0000a1c0: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 0000a1d0: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 0000a1e0: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 0000a1f0: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 0000a200: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 0000a210: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 0000a220: 6532 645f 3634 223e 0a20 2020 203c 7061  e2d_64">.    <pa
 0000a230: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-0000a240: 6c28 2370 3232 6131 3661 3664 6264 2922  l(#p22a16a6dbd)"
+0000a240: 6c28 2370 3234 6234 6338 3065 3839 2922  l(#p24b4c80e89)"
 0000a250: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 0000a260: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 0000a270: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 0000a280: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 0000a290: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 0000a2a0: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 0000a2b0: 6964 3d22 6c69 6e65 3264 5f36 3522 3e0a  id="line2d_65">.
 0000a2c0: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-0000a2d0: 6174 683d 2275 726c 2823 7032 3261 3136  ath="url(#p22a16
-0000a2e0: 6136 6462 6429 2220 7374 796c 653d 2266  a6dbd)" style="f
+0000a2d0: 6174 683d 2275 726c 2823 7032 3462 3463  ath="url(#p24b4c
+0000a2e0: 3830 6538 3929 2220 7374 796c 653d 2266  80e89)" style="f
 0000a2f0: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 0000a300: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 0000a310: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 0000a320: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 0000a330: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 0000a340: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 0000a350: 645f 3636 223e 0a20 2020 203c 7061 7468  d_66">.    <path
 0000a360: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000a370: 2370 3232 6131 3661 3664 6264 2922 2073  #p22a16a6dbd)" s
+0000a370: 2370 3234 6234 6338 3065 3839 2922 2073  #p24b4c80e89)" s
 0000a380: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 0000a390: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 0000a3a0: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 0000a3b0: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 0000a3c0: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 0000a3d0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0000a3e0: 3d22 6c69 6e65 3264 5f36 3722 3e0a 2020  ="line2d_67">.  
 0000a3f0: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-0000a400: 683d 2275 726c 2823 7032 3261 3136 6136  h="url(#p22a16a6
-0000a410: 6462 6429 2220 7374 796c 653d 2266 696c  dbd)" style="fil
+0000a400: 683d 2275 726c 2823 7032 3462 3463 3830  h="url(#p24b4c80
+0000a410: 6538 3929 2220 7374 796c 653d 2266 696c  e89)" style="fil
 0000a420: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 0000a430: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 0000a440: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 0000a450: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 0000a460: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 0000a470: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 0000a480: 3638 223e 0a20 2020 203c 7061 7468 2063  68">.    <path c
 0000a490: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-0000a4a0: 3232 6131 3661 3664 6264 2922 2073 7479  22a16a6dbd)" sty
+0000a4a0: 3234 6234 6338 3065 3839 2922 2073 7479  24b4c80e89)" sty
 0000a4b0: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 0000a4c0: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 0000a4d0: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 0000a4e0: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 0000a4f0: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 0000a500: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 0000a510: 7061 7463 685f 3333 223e 0a20 2020 203c  patch_33">.    <
@@ -3007,15 +3007,15 @@
 0000bbe0: 392e 3936 3837 3522 2f3e 0a20 2020 2020  9.96875"/>.     
 0000bbf0: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000bc00: 2223 4465 6a61 5675 5361 6e73 2d37 3322  "#DejaVuSans-73"
 0000bc10: 2078 3d22 3231 3931 2e34 3932 3138 3822   x="2191.492188"
 0000bc20: 2f3e 0a20 2020 203c 2f67 3e0a 2020 203c  />.    </g>.   <
 0000bc30: 2f67 3e0a 2020 3c2f 673e 0a20 3c2f 673e  /g>.  </g>. </g>
 0000bc40: 0a20 3c64 6566 733e 0a20 203c 636c 6970  . <defs>.  <clip
-0000bc50: 5061 7468 2069 643d 2270 3232 6131 3661  Path id="p22a16a
-0000bc60: 3664 6264 223e 0a20 2020 3c72 6563 7420  6dbd">.   <rect 
+0000bc50: 5061 7468 2069 643d 2270 3234 6234 6338  Path id="p24b4c8
+0000bc60: 3065 3839 223e 0a20 2020 3c72 6563 7420  0e89">.   <rect 
 0000bc70: 783d 2234 342e 3537 2220 793d 2232 362e  x="44.57" y="26.
 0000bc80: 3838 2220 7769 6474 683d 2235 3135 2e35  88" width="515.5
 0000bc90: 3936 3633 3622 2068 6569 6768 743d 2231  96636" height="1
 0000bca0: 3832 2e31 3138 3731 3422 2f3e 0a20 203c  82.118714"/>.  <
 0000bcb0: 2f63 6c69 7050 6174 683e 0a20 3c2f 6465  /clipPath>. </de
 0000bcc0: 6673 3e0a 3c2f 7376 673e 0a              fs>.</svg>.
```

### Comparing `bioregistry-0.9.7/docs/img/bioregistry_coverage.svg` & `bioregistry-0.9.8/docs/img/bioregistry_coverage.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6178 2d6e 7323 223e 0a20 2020 3c63 633a  ax-ns#">.   <cc:
 000001e0: 576f 726b 3e0a 2020 2020 3c64 633a 7479  Work>.    <dc:ty
 000001f0: 7065 2072 6466 3a72 6573 6f75 7263 653d  pe rdf:resource=
 00000200: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
 00000210: 2f64 632f 6463 6d69 7479 7065 2f53 7469  /dc/dcmitype/Sti
 00000220: 6c6c 496d 6167 6522 2f3e 0a20 2020 203c  llImage"/>.    <
 00000230: 6463 3a64 6174 653e 3230 3233 2d30 352d  dc:date>2023-05-
-00000240: 3037 5430 313a 3134 3a30 382e 3138 3238  07T01:14:08.1828
-00000250: 3035 3c2f 6463 3a64 6174 653e 0a20 2020  05</dc:date>.   
+00000240: 3038 5430 313a 3037 3a31 322e 3737 3739  08T01:07:12.7779
+00000250: 3330 3c2f 6463 3a64 6174 653e 0a20 2020  30</dc:date>.   
 00000260: 203c 6463 3a66 6f72 6d61 743e 696d 6167   <dc:format>imag
 00000270: 652f 7376 672b 786d 6c3c 2f64 633a 666f  e/svg+xml</dc:fo
 00000280: 726d 6174 3e0a 2020 2020 3c64 633a 6372  rmat>.    <dc:cr
 00000290: 6561 746f 723e 0a20 2020 2020 3c63 633a  eator>.     <cc:
 000002a0: 4167 656e 743e 0a20 2020 2020 203c 6463  Agent>.      <dc
 000002b0: 3a74 6974 6c65 3e4d 6174 706c 6f74 6c69  :title>Matplotli
 000002c0: 6220 7633 2e37 2e31 2c20 6874 7470 733a  b v3.7.1, https:
@@ -9350,15 +9350,15 @@
 00024850: 3930 3632 222f 3e0a 2020 2020 3c2f 673e  9062"/>.    </g>
 00024860: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 00024870: 2020 3c67 2069 643d 2274 6578 745f 3132    <g id="text_12
 00024880: 3122 3e0a 2020 203c 212d 2d20 6874 7470  1">.   <!-- http
 00024890: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
 000248a0: 696f 7072 6167 6d61 7469 6373 2f62 696f  iopragmatics/bio
 000248b0: 7265 6769 7374 7279 2028 3230 3233 2d30  registry (2023-0
-000248c0: 352d 3037 2920 2d2d 3e0a 2020 203c 6720  5-07) -->.   <g 
+000248c0: 352d 3038 2920 2d2d 3e0a 2020 203c 6720  5-08) -->.   <g 
 000248d0: 7374 796c 653d 2266 696c 6c3a 2023 3830  style="fill: #80
 000248e0: 3830 3830 3b20 6f70 6163 6974 793a 2030  8080; opacity: 0
 000248f0: 2e35 2220 7472 616e 7366 6f72 6d3d 2274  .5" transform="t
 00024900: 7261 6e73 6c61 7465 2832 3333 2e36 3736  ranslate(233.676
 00024910: 3235 2031 3135 302e 3333 3632 3529 2073  25 1150.33625) s
 00024920: 6361 6c65 2830 2e30 3820 2d30 2e30 3829  cale(0.08 -0.08)
 00024930: 223e 0a20 2020 203c 6465 6673 3e0a 2020  ">.    <defs>.  
@@ -9617,15 +9617,15 @@
 00025900: 5675 5361 6e73 2d32 6422 2078 3d22 3237  VuSans-2d" x="27
 00025910: 3330 2e37 3537 3831 3222 2f3e 0a20 2020  30.757812"/>.   
 00025920: 203c 7573 6520 786c 696e 6b3a 6872 6566   <use xlink:href
 00025930: 3d22 2344 656a 6156 7553 616e 732d 3330  ="#DejaVuSans-30
 00025940: 2220 783d 2232 3736 362e 3834 3137 3937  " x="2766.841797
 00025950: 222f 3e0a 2020 2020 3c75 7365 2078 6c69  "/>.    <use xli
 00025960: 6e6b 3a68 7265 663d 2223 4465 6a61 5675  nk:href="#DejaVu
-00025970: 5361 6e73 2d33 3722 2078 3d22 3238 3330  Sans-37" x="2830
+00025970: 5361 6e73 2d33 3822 2078 3d22 3238 3330  Sans-38" x="2830
 00025980: 2e34 3634 3834 3422 2f3e 0a20 2020 203c  .464844"/>.    <
 00025990: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 000259a0: 2344 656a 6156 7553 616e 732d 3239 2220  #DejaVuSans-29" 
 000259b0: 783d 2232 3839 342e 3038 3738 3931 222f  x="2894.087891"/
 000259c0: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 000259d0: 0a20 3c2f 673e 0a20 3c64 6566 733e 0a20  . </g>. <defs>. 
 000259e0: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
```

### Comparing `bioregistry-0.9.7/docs/img/bioregistry_coverage_bar.svg` & `bioregistry-0.9.8/docs/img/bioregistry_coverage_bar.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3134 3a30 372e 3035 3932 3935  T01:14:07.059295
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3037 3a31 312e 3931 3932 3430  T01:07:11.919240
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.7/docs/img/bioregistry_coverage_bar_short.svg` & `bioregistry-0.9.8/docs/img/bioregistry_coverage_bar_short.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3134 3a30 382e 3538 3130 3532  T01:14:08.581052
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3037 3a31 332e 3039 3032 3630  T01:07:13.090260
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.7/docs/img/datamodel_umls.svg` & `bioregistry-0.9.8/docs/img/datamodel_umls.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/docs/img/external_overlap.svg` & `bioregistry-0.9.8/docs/img/external_overlap.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6e74 6178 2d6e 7323 223e 0a20 2020 3c63  ntax-ns#">.   <c
 000001e0: 633a 576f 726b 3e0a 2020 2020 3c64 633a  c:Work>.    <dc:
 000001f0: 7479 7065 2072 6466 3a72 6573 6f75 7263  type rdf:resourc
 00000200: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
 00000210: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
 00000220: 7469 6c6c 496d 6167 6522 2f3e 0a20 2020  tillImage"/>.   
 00000230: 203c 6463 3a64 6174 653e 3230 3233 2d30   <dc:date>2023-0
-00000240: 352d 3037 5430 313a 3138 3a30 332e 3232  5-07T01:18:03.22
-00000250: 3034 3933 3c2f 6463 3a64 6174 653e 0a20  0493</dc:date>. 
+00000240: 352d 3038 5430 313a 3130 3a34 332e 3436  5-08T01:10:43.46
+00000250: 3639 3431 3c2f 6463 3a64 6174 653e 0a20  6941</dc:date>. 
 00000260: 2020 203c 6463 3a66 6f72 6d61 743e 696d     <dc:format>im
 00000270: 6167 652f 7376 672b 786d 6c3c 2f64 633a  age/svg+xml</dc:
 00000280: 666f 726d 6174 3e0a 2020 2020 3c64 633a  format>.    <dc:
 00000290: 6372 6561 746f 723e 0a20 2020 2020 3c63  creator>.     <c
 000002a0: 633a 4167 656e 743e 0a20 2020 2020 203c  c:Agent>.      <
 000002b0: 6463 3a74 6974 6c65 3e4d 6174 706c 6f74  dc:title>Matplot
 000002c0: 6c69 6220 7633 2e37 2e31 2c20 6874 7470  lib v3.7.1, http
@@ -83950,15 +83950,15 @@
 00147ed0: 3339 3036 3222 2f3e 0a20 2020 203c 2f67  39062"/>.    </g
 00147ee0: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 00147ef0: 0a20 203c 6720 6964 3d22 7465 7874 5f31  .  <g id="text_1
 00147f00: 3334 3822 3e0a 2020 203c 212d 2d20 6874  348">.   <!-- ht
 00147f10: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00147f20: 2f62 696f 7072 6167 6d61 7469 6373 2f62  /biopragmatics/b
 00147f30: 696f 7265 6769 7374 7279 2028 3230 3233  ioregistry (2023
-00147f40: 2d30 352d 3037 2920 2d2d 3e0a 2020 203c  -05-07) -->.   <
+00147f40: 2d30 352d 3038 2920 2d2d 3e0a 2020 203c  -05-08) -->.   <
 00147f50: 6720 7374 796c 653d 2266 696c 6c3a 2023  g style="fill: #
 00147f60: 3830 3830 3830 3b20 6f70 6163 6974 793a  808080; opacity:
 00147f70: 2030 2e35 2220 7472 616e 7366 6f72 6d3d   0.5" transform=
 00147f80: 2274 7261 6e73 6c61 7465 2832 3236 2e36  "translate(226.6
 00147f90: 3833 3433 3720 3132 3431 372e 3038 3834  83437 12417.0884
 00147fa0: 3338 2920 7363 616c 6528 302e 3134 202d  38) scale(0.14 -
 00147fb0: 302e 3134 2922 3e0a 2020 2020 3c64 6566  0.14)">.    <def
@@ -84236,15 +84236,15 @@
 001490b0: 5361 6e73 2d32 6422 2078 3d22 3237 3330  Sans-2d" x="2730
 001490c0: 2e37 3537 3831 3222 2f3e 0a20 2020 203c  .757812"/>.    <
 001490d0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 001490e0: 2344 656a 6156 7553 616e 732d 3330 2220  #DejaVuSans-30" 
 001490f0: 783d 2232 3736 362e 3834 3137 3937 222f  x="2766.841797"/
 00149100: 3e0a 2020 2020 3c75 7365 2078 6c69 6e6b  >.    <use xlink
 00149110: 3a68 7265 663d 2223 4465 6a61 5675 5361  :href="#DejaVuSa
-00149120: 6e73 2d33 3722 2078 3d22 3238 3330 2e34  ns-37" x="2830.4
+00149120: 6e73 2d33 3822 2078 3d22 3238 3330 2e34  ns-38" x="2830.4
 00149130: 3634 3834 3422 2f3e 0a20 2020 203c 7573  64844"/>.    <us
 00149140: 6520 786c 696e 6b3a 6872 6566 3d22 2344  e xlink:href="#D
 00149150: 656a 6156 7553 616e 732d 3239 2220 783d  ejaVuSans-29" x=
 00149160: 2232 3839 342e 3038 3738 3931 222f 3e0a  "2894.087891"/>.
 00149170: 2020 203c 2f67 3e0a 2020 3c2f 673e 0a20     </g>.  </g>. 
 00149180: 3c2f 673e 0a20 3c64 6566 733e 0a20 203c  </g>. <defs>.  <
 00149190: 636c 6970 5061 7468 2069 643d 2270 6461  clipPath id="pda
```

### Comparing `bioregistry-0.9.7/docs/img/has_attribute.svg` & `bioregistry-0.9.8/docs/img/has_attribute.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3134 3a33 352e 3231 3138 3337  T01:14:35.211837
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3037 3a33 362e 3837 3035 3033  T01:07:36.870503
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -4243,15 +4243,15 @@
 00010920: 3c2f 673e 0a20 203c 6720 6964 3d22 6178  </g>.  <g id="ax
 00010930: 6573 5f31 3522 2f3e 0a20 203c 6720 6964  es_15"/>.  <g id
 00010940: 3d22 6178 6573 5f31 3622 2f3e 0a20 203c  ="axes_16"/>.  <
 00010950: 6720 6964 3d22 7465 7874 5f37 3522 3e0a  g id="text_75">.
 00010960: 2020 203c 212d 2d20 6874 7470 733a 2f2f     <!-- https://
 00010970: 6769 7468 7562 2e63 6f6d 2f62 696f 7072  github.com/biopr
 00010980: 6167 6d61 7469 6373 2f62 696f 7265 6769  agmatics/bioregi
-00010990: 7374 7279 2028 3230 3233 2d30 352d 3037  stry (2023-05-07
+00010990: 7374 7279 2028 3230 3233 2d30 352d 3038  stry (2023-05-08
 000109a0: 2920 2d2d 3e0a 2020 203c 6720 7374 796c  ) -->.   <g styl
 000109b0: 653d 2266 696c 6c3a 2023 3830 3830 3830  e="fill: #808080
 000109c0: 3b20 6f70 6163 6974 793a 2030 2e35 2220  ; opacity: 0.5" 
 000109d0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
 000109e0: 6c61 7465 2832 3738 2e36 3736 3235 2035  late(278.67625 5
 000109f0: 3734 2e33 3336 3235 2920 7363 616c 6528  74.33625) scale(
 00010a00: 302e 3038 202d 302e 3038 2922 3e0a 2020  0.08 -0.08)">.  
@@ -4518,15 +4518,15 @@
 00011a50: 4465 6a61 5675 5361 6e73 2d32 6422 2078  DejaVuSans-2d" x
 00011a60: 3d22 3237 3330 2e37 3537 3831 3222 2f3e  ="2730.757812"/>
 00011a70: 0a20 2020 203c 7573 6520 786c 696e 6b3a  .    <use xlink:
 00011a80: 6872 6566 3d22 2344 656a 6156 7553 616e  href="#DejaVuSan
 00011a90: 732d 3330 2220 783d 2232 3736 362e 3834  s-30" x="2766.84
 00011aa0: 3137 3937 222f 3e0a 2020 2020 3c75 7365  1797"/>.    <use
 00011ab0: 2078 6c69 6e6b 3a68 7265 663d 2223 4465   xlink:href="#De
-00011ac0: 6a61 5675 5361 6e73 2d33 3722 2078 3d22  jaVuSans-37" x="
+00011ac0: 6a61 5675 5361 6e73 2d33 3822 2078 3d22  jaVuSans-38" x="
 00011ad0: 3238 3330 2e34 3634 3834 3422 2f3e 0a20  2830.464844"/>. 
 00011ae0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
 00011af0: 6566 3d22 2344 656a 6156 7553 616e 732d  ef="#DejaVuSans-
 00011b00: 3239 2220 783d 2232 3839 342e 3038 3738  29" x="2894.0878
 00011b10: 3931 222f 3e0a 2020 203c 2f67 3e0a 2020  91"/>.   </g>.  
 00011b20: 3c2f 673e 0a20 3c2f 673e 0a3c 2f73 7667  </g>. </g>.</svg
 00011b30: 3e0a                                     >.
```

### Comparing `bioregistry-0.9.7/docs/img/providers.svg` & `bioregistry-0.9.8/docs/img/providers.svg`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3138 3a30 362e 3137 3333 3633  T01:18:06.173363
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3130 3a34 352e 3839 3630 3038  T01:10:45.896008
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -1304,15 +1304,15 @@
 00005170: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00005180: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00005190: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
 000051a0: 6964 3d22 7465 7874 5f31 3522 3e0a 2020  id="text_15">.  
 000051b0: 203c 212d 2d20 6874 7470 733a 2f2f 6769   <!-- https://gi
 000051c0: 7468 7562 2e63 6f6d 2f62 696f 7072 6167  thub.com/bioprag
 000051d0: 6d61 7469 6373 2f62 696f 7265 6769 7374  matics/bioregist
-000051e0: 7279 2028 3230 3233 2d30 352d 3037 2920  ry (2023-05-07) 
+000051e0: 7279 2028 3230 3233 2d30 352d 3038 2920  ry (2023-05-08) 
 000051f0: 2d2d 3e0a 2020 203c 6720 7374 796c 653d  -->.   <g style=
 00005200: 2266 696c 6c3a 2023 3830 3830 3830 3b20  "fill: #808080; 
 00005210: 6f70 6163 6974 793a 2030 2e35 2220 7472  opacity: 0.5" tr
 00005220: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
 00005230: 7465 2835 3932 2e33 3336 3235 2032 3433  te(592.33625 243
 00005240: 2e33 3233 3735 2920 726f 7461 7465 282d  .32375) rotate(-
 00005250: 3930 2920 7363 616c 6528 302e 3038 202d  90) scale(0.08 -
@@ -1755,15 +1755,15 @@
 00006da0: 656a 6156 7553 616e 732d 3264 2220 783d  ejaVuSans-2d" x=
 00006db0: 2232 3733 302e 3735 3738 3132 222f 3e0a  "2730.757812"/>.
 00006dc0: 2020 2020 3c75 7365 2078 6c69 6e6b 3a68      <use xlink:h
 00006dd0: 7265 663d 2223 4465 6a61 5675 5361 6e73  ref="#DejaVuSans
 00006de0: 2d33 3022 2078 3d22 3237 3636 2e38 3431  -30" x="2766.841
 00006df0: 3739 3722 2f3e 0a20 2020 203c 7573 6520  797"/>.    <use 
 00006e00: 786c 696e 6b3a 6872 6566 3d22 2344 656a  xlink:href="#Dej
-00006e10: 6156 7553 616e 732d 3337 2220 783d 2232  aVuSans-37" x="2
+00006e10: 6156 7553 616e 732d 3338 2220 783d 2232  aVuSans-38" x="2
 00006e20: 3833 302e 3436 3438 3434 222f 3e0a 2020  830.464844"/>.  
 00006e30: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
 00006e40: 663d 2223 4465 6a61 5675 5361 6e73 2d32  f="#DejaVuSans-2
 00006e50: 3922 2078 3d22 3238 3934 2e30 3837 3839  9" x="2894.08789
 00006e60: 3122 2f3e 0a20 2020 3c2f 673e 0a20 203c  1"/>.   </g>.  <
 00006e70: 2f67 3e0a 203c 2f67 3e0a 203c 6465 6673  /g>. </g>. <defs
 00006e80: 3e0a 2020 3c63 6c69 7050 6174 6820 6964  >.  <clipPath id
```

### Comparing `bioregistry-0.9.7/docs/img/regex_report.svg` & `bioregistry-0.9.8/docs/img/regex_report.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3138 3a30 372e 3131 3036 3636  T01:18:07.110666
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3130 3a34 362e 3731 3432 3234  T01:10:46.714224
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.7/docs/img/xrefs.svg` & `bioregistry-0.9.8/docs/img/xrefs.svg`

 * *Files identical despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3037  :date>2023-05-07
-00000240: 5430 313a 3134 3a30 362e 3635 3932 3031  T01:14:06.659201
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3038  :date>2023-05-08
+00000240: 5430 313a 3037 3a31 312e 3631 3036 3037  T01:07:11.610607
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -2920,15 +2920,15 @@
 0000b670: 352e 3638 3535 3437 222f 3e0a 2020 2020  5.685547"/>.    
 0000b680: 3c2f 673e 0a20 2020 3c2f 673e 0a20 203c  </g>.   </g>.  <
 0000b690: 2f67 3e0a 2020 3c67 2069 643d 2274 6578  /g>.  <g id="tex
 0000b6a0: 745f 3438 223e 0a20 2020 3c21 2d2d 2068  t_48">.   <!-- h
 0000b6b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0000b6c0: 6d2f 6269 6f70 7261 676d 6174 6963 732f  m/biopragmatics/
 0000b6d0: 6269 6f72 6567 6973 7472 7920 2832 3032  bioregistry (202
-0000b6e0: 332d 3035 2d30 3729 202d 2d3e 0a20 2020  3-05-07) -->.   
+0000b6e0: 332d 3035 2d30 3829 202d 2d3e 0a20 2020  3-05-08) -->.   
 0000b6f0: 3c67 2073 7479 6c65 3d22 6669 6c6c 3a20  <g style="fill: 
 0000b700: 2338 3038 3038 303b 206f 7061 6369 7479  #808080; opacity
 0000b710: 3a20 302e 3522 2074 7261 6e73 666f 726d  : 0.5" transform
 0000b720: 3d22 7472 616e 736c 6174 6528 3539 322e  ="translate(592.
 0000b730: 3333 3632 3520 3234 332e 3332 3337 3529  33625 243.32375)
 0000b740: 2072 6f74 6174 6528 2d39 3029 2073 6361   rotate(-90) sca
 0000b750: 6c65 2830 2e30 3820 2d30 2e30 3829 223e  le(0.08 -0.08)">
@@ -3199,15 +3199,15 @@
 0000c7e0: 7553 616e 732d 3264 2220 783d 2232 3733  uSans-2d" x="273
 0000c7f0: 302e 3735 3738 3132 222f 3e0a 2020 2020  0.757812"/>.    
 0000c800: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000c810: 2223 4465 6a61 5675 5361 6e73 2d33 3022  "#DejaVuSans-30"
 0000c820: 2078 3d22 3237 3636 2e38 3431 3739 3722   x="2766.841797"
 0000c830: 2f3e 0a20 2020 203c 7573 6520 786c 696e  />.    <use xlin
 0000c840: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
-0000c850: 616e 732d 3337 2220 783d 2232 3833 302e  ans-37" x="2830.
+0000c850: 616e 732d 3338 2220 783d 2232 3833 302e  ans-38" x="2830.
 0000c860: 3436 3438 3434 222f 3e0a 2020 2020 3c75  464844"/>.    <u
 0000c870: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
 0000c880: 4465 6a61 5675 5361 6e73 2d32 3922 2078  DejaVuSans-29" x
 0000c890: 3d22 3238 3934 2e30 3837 3839 3122 2f3e  ="2894.087891"/>
 0000c8a0: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 0000c8b0: 203c 2f67 3e0a 203c 6465 6673 3e0a 2020   </g>. <defs>.  
 0000c8c0: 3c63 6c69 7050 6174 6820 6964 3d22 7031  <clipPath id="p1
```

### Comparing `bioregistry-0.9.7/docs/source/conf.py` & `bioregistry-0.9.8/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "bioregistry"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.9.7"
+release = "0.9.8"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `bioregistry-0.9.7/docs/source/deployment.rst` & `bioregistry-0.9.8/docs/source/deployment.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/docs/source/index.rst` & `bioregistry-0.9.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/docs/source/logo.png` & `bioregistry-0.9.8/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/setup.cfg` & `bioregistry-0.9.8/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bioregistry
-version = 0.9.7
+version = 0.9.8
 description = Integrated registry of biological databases and nomenclatures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioregistry
 download_url = https://github.com/biopragmatics/bioregistry/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioregistry/issues
```

### Comparing `bioregistry-0.9.7/src/bioregistry/__init__.py` & `bioregistry-0.9.8/src/bioregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/__init__.py` & `bioregistry-0.9.8/src/bioregistry/align/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/biocontext.py` & `bioregistry-0.9.8/src/bioregistry/align/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/biolink.py` & `bioregistry-0.9.8/src/bioregistry/align/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/bioportal.py` & `bioregistry-0.9.8/src/bioregistry/align/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/cellosaurus.py` & `bioregistry-0.9.8/src/bioregistry/align/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/cheminf.py` & `bioregistry-0.9.8/src/bioregistry/align/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/edam.py` & `bioregistry-0.9.8/src/bioregistry/align/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/fairsharing.py` & `bioregistry-0.9.8/src/bioregistry/align/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/go.py` & `bioregistry-0.9.8/src/bioregistry/align/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/hl7.py` & `bioregistry-0.9.8/src/bioregistry/align/hl7.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/n2t.py` & `bioregistry-0.9.8/src/bioregistry/align/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/ncbi.py` & `bioregistry-0.9.8/src/bioregistry/align/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/obofoundry.py` & `bioregistry-0.9.8/src/bioregistry/align/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/ols.py` & `bioregistry-0.9.8/src/bioregistry/align/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/ontobee.py` & `bioregistry-0.9.8/src/bioregistry/align/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/prefixcommons.py` & `bioregistry-0.9.8/src/bioregistry/align/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/re3data.py` & `bioregistry-0.9.8/src/bioregistry/align/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/uniprot.py` & `bioregistry-0.9.8/src/bioregistry/align/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/utils.py` & `bioregistry-0.9.8/src/bioregistry/align/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/align/wikidata.py` & `bioregistry-0.9.8/src/bioregistry/align/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/analysis/title_tfidf.py` & `bioregistry-0.9.8/src/bioregistry/analysis/title_tfidf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/api.py` & `bioregistry-0.9.8/src/bioregistry/app/api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/cli.py` & `bioregistry-0.9.8/src/bioregistry/app/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/constants.py` & `bioregistry-0.9.8/src/bioregistry/app/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/impl.py` & `bioregistry-0.9.8/src/bioregistry/app/impl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/static/logo.svg` & `bioregistry-0.9.8/src/bioregistry/app/static/logo.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/base.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/collection.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/collection.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/collections.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/collections.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/context.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/context.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/contexts.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/contexts.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/contributor.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/contributor.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/contributors.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/contributors.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/keywords.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/highlights/keywords.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/owners.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/highlights/owners.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/relations.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/highlights/relations.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/highlights/twitter.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/highlights/twitter.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/home.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/home.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/macros.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/macros.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/access.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/access.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/acknowledgements.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/acknowledgements.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/download.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/download.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/related.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/related.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/schema.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/schema.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/summary.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/summary.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/meta/sustainability.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/meta/sustainability.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/metaresource.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/metaresource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/metaresources.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/metaresources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/prose.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/prose.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/reference.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/reference.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_prefix.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/missing_prefix.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resolve_errors/missing_providers.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resolve_errors/missing_providers.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resource.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/templates/resources.html` & `bioregistry-0.9.8/src/bioregistry/app/templates/resources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/test.py` & `bioregistry-0.9.8/src/bioregistry/app/test.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/ui.py` & `bioregistry-0.9.8/src/bioregistry/app/ui.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/app/utils.py` & `bioregistry-0.9.8/src/bioregistry/app/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/benchmarks/cli.py` & `bioregistry-0.9.8/src/bioregistry/benchmarks/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/benchmarks/curie_parsing.py` & `bioregistry-0.9.8/src/bioregistry/benchmarks/curie_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/benchmarks/curie_validation.py` & `bioregistry-0.9.8/src/bioregistry/benchmarks/curie_validation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/benchmarks/uri_parsing.py` & `bioregistry-0.9.8/src/bioregistry/benchmarks/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/bibliometrics.py` & `bioregistry-0.9.8/src/bioregistry/bibliometrics.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/cli.py` & `bioregistry-0.9.8/src/bioregistry/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/collection_api.py` & `bioregistry-0.9.8/src/bioregistry/collection_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/compare.py` & `bioregistry-0.9.8/src/bioregistry/compare.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/constants.py` & `bioregistry-0.9.8/src/bioregistry/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_co_providers.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_co_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_descriptions_from_gs.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_descriptions_from_gs.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_examples.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_examples.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_javert.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_examples_from_javert.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_examples_from_ols.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_examples_from_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/add_ontology_regexes.py` & `bioregistry-0.9.8/src/bioregistry/curation/add_ontology_regexes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/bulk_import.py` & `bioregistry-0.9.8/src/bioregistry/curation/bulk_import.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/clean_licenses.py` & `bioregistry-0.9.8/src/bioregistry/curation/clean_licenses.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/clean_name_suffixes.py` & `bioregistry-0.9.8/src/bioregistry/curation/clean_name_suffixes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/clean_publications.py` & `bioregistry-0.9.8/src/bioregistry/curation/clean_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/cleanup_authors.py` & `bioregistry-0.9.8/src/bioregistry/curation/cleanup_authors.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/deprecation_diff.py` & `bioregistry-0.9.8/src/bioregistry/curation/deprecation_diff.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/enrich_publications.py` & `bioregistry-0.9.8/src/bioregistry/curation/enrich_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/import_pc_semiautomatic.py` & `bioregistry-0.9.8/src/bioregistry/curation/import_pc_semiautomatic.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/make_description_curation_sheet.py` & `bioregistry-0.9.8/src/bioregistry/curation/make_description_curation_sheet.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/map_bartoc_via_wikidata.py` & `bioregistry-0.9.8/src/bioregistry/curation/map_bartoc_via_wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/map_re3data_via_fairsharing.py` & `bioregistry-0.9.8/src/bioregistry/curation/map_re3data_via_fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/rename_metaprefix.py` & `bioregistry-0.9.8/src/bioregistry/curation/rename_metaprefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/review_pc.py` & `bioregistry-0.9.8/src/bioregistry/curation/review_pc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/suggest_author_curation.py` & `bioregistry-0.9.8/src/bioregistry/curation/suggest_author_curation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/curation/suggest_uniprot_providers.py` & `bioregistry-0.9.8/src/bioregistry/curation/suggest_uniprot_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/README.md` & `bioregistry-0.9.8/src/bioregistry/data/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/bioregistry.json` & `bioregistry-0.9.8/src/bioregistry/data/bioregistry.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/collections.json` & `bioregistry-0.9.8/src/bioregistry/data/collections.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/contexts.json` & `bioregistry-0.9.8/src/bioregistry/data/contexts.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/aberowl/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/aberowl/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/aberowl/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/aberowl/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/agroportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/agroportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/agroportal/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/agroportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/bartoc/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/bartoc/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/bartoc/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/bartoc/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/biocontext/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/biocontext/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biocontext/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/biocontext/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biolink/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/biolink/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biolink/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/biolink/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/biolink/raw.yaml` & `bioregistry-0.9.8/src/bioregistry/data/external/biolink/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/bioportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/bioportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/bioportal/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/bioportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cellosaurus/raw.txt` & `bioregistry-0.9.8/src/bioregistry/data/external/cellosaurus/raw.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cheminf/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/cheminf/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cropoct/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/cropoct/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/cropoct/raw.yaml` & `bioregistry-0.9.8/src/bioregistry/data/external/cropoct/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ecoportal/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ecoportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/edam/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/edam/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/edam/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/edam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/fairsharing/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/fairsharing/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/go/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/go/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/go/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/go/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/go/raw.yml` & `bioregistry-0.9.8/src/bioregistry/data/external/go/raw.yml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/hl7/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/hl7/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/miriam/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/miriam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/miriam/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/miriam/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/n2t/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/n2t/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/n2t/raw.yml` & `bioregistry-0.9.8/src/bioregistry/data/external/n2t/raw.yml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/ncbi/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ncbi/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.8/src/bioregistry/data/external/ncbi/raw.html`

 * *Files 0% similar despite different names*

#### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.8/src/bioregistry/data/external/ncbi/raw.html`

```diff
@@ -30,15 +30,15 @@
     <meta name="modified" content="2021-10-25T17:46:25Z"/>
     <meta xmlns:ncbi-portal="http://ncbi.gov/portal/XSLT/namespace" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" name="cms-edit-aux-url" content="http://cms.ncbi.nlm.nih.gov/node//edit"/>
     <!-- Page headcontent end -->
     <!-- PageFixtures resources begin -->
     <link xmlns="http://www.w3.org/1999/xhtml" type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4208398/css/4207974/4206132.css" xml:base="http://127.0.0.1/sites/static/header_footer"/>
     <!-- PageFixtures resources end -->
     <link rel="shortcut icon" href="//www.ncbi.nlm.nih.gov/favicon.ico"/>
-    <meta name="ncbi_phid" content="CE884B84456D0B610000000004F8035B.m_6"/>
+    <meta name="ncbi_phid" content="CE882F03458137C10000000007880599.m_5"/>
     <meta name="referrer" content="origin-when-cross-origin"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/4121862/3974050/3917732/251717/4108189/14534/45193/3534283/4128070/3407145/4005757/4062871.css"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/3529741/3529739.css" media="print"/>
   </head>
   <body class=" col2  custom-page">
     <div class="grid">
       <div class="col twelve_col nomargin shadow">
@@ -3248,17 +3248,17 @@
             <div id="NCBIFooter_dynamic">
               <div class="breadcrumbs">
                 You are here:
                 <span id="breadcrumb_text">
                   <a href="/guide/">NCBI</a>
                 </span>
               </div>
-              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-06T21:04:42-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal101&amp;ncbi_phid=CE884B84456D0B610000000004F8035B&amp;ncbi_session=CE884B84456F92A1_1272SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
+              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-07T20:59:35-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal101&amp;ncbi_phid=CE882F03458137C10000000007880599&amp;ncbi_session=CE882F0345849771_1928SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
               <noscript>
-                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE884B84456D0B610000000004F8035B"/>
+                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE882F03458137C10000000007880599"/>
               </noscript>
             </div>
             <div xmlns:xi="http://www.w3.org/2001/XInclude">
               <div xmlns="http://www.w3.org/1999/xhtml" class="footer" id="footer" xml:base="http://127.0.0.1/sites/static/header_footer">
                 <section class="icon-section">
                   <div id="icon-section-header" class="icon-section_header">Follow NCBI</div>
                   <div class="grid-container container">
@@ -3465,12 +3465,12 @@
         <span class="PAFAppResources"/>
       </div>
       <!-- /.twelve_col -->
     </div>
     <!-- /.grid -->
     <!-- usually for JS scripts at page bottom -->
     <span class="pagefixtures"/>
-    <!-- CE884B84456F92A1_1272SID /projects/staticsites/genbank/genbank@2.20 portal101 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
-    <span id="portal-csrf-token" style="display:none" data-token="CE884B84456F92A1_1272SID"/>
+    <!-- CE882F0345849771_1928SID /projects/staticsites/genbank/genbank@2.20 portal101 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
+    <span id="portal-csrf-token" style="display:none" data-token="CE882F0345849771_1928SID"/>
     <script type="text/javascript" src="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/js/3879255/4121861/1490097/4087685.js" snapshot="genbank"/>
   </body>
 </html>
```

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/obofoundry/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/obofoundry/raw.yaml` & `bioregistry-0.9.8/src/bioregistry/data/external/obofoundry/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ols/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ols/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ols/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ols/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/ontobee/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/ontobee/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/ontobee/raw.html` & `bioregistry-0.9.8/src/bioregistry/data/external/ontobee/raw.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/prefixcommons/raw.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/prefixcommons/raw.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/re3data/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/re3data/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/re3data/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/re3data/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/uniprot/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/uniprot/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/uniprot/raw.json` & `bioregistry-0.9.8/src/bioregistry/data/external/uniprot/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/wikidata/curation.tsv` & `bioregistry-0.9.8/src/bioregistry/data/external/wikidata/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/external/wikidata/processed.json` & `bioregistry-0.9.8/src/bioregistry/data/external/wikidata/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/metaregistry.json` & `bioregistry-0.9.8/src/bioregistry/data/metaregistry.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/mismatch.json` & `bioregistry-0.9.8/src/bioregistry/data/mismatch.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/data/processing_ols.json` & `bioregistry-0.9.8/src/bioregistry/data/processing_ols.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/cli.py` & `bioregistry-0.9.8/src/bioregistry/export/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/prefix_maps.py` & `bioregistry-0.9.8/src/bioregistry/export/prefix_maps.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/rdf_export.py` & `bioregistry-0.9.8/src/bioregistry/export/rdf_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/sssom_export.py` & `bioregistry-0.9.8/src/bioregistry/export/sssom_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/tables_export.py` & `bioregistry-0.9.8/src/bioregistry/export/tables_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/tsv_export.py` & `bioregistry-0.9.8/src/bioregistry/export/tsv_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/warnings_export.py` & `bioregistry-0.9.8/src/bioregistry/export/warnings_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/export/yaml_export.py` & `bioregistry-0.9.8/src/bioregistry/export/yaml_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/__init__.py` & `bioregistry-0.9.8/src/bioregistry/external/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/aberowl.py` & `bioregistry-0.9.8/src/bioregistry/external/aberowl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/bartoc.py` & `bioregistry-0.9.8/src/bioregistry/external/bartoc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/biocontext.py` & `bioregistry-0.9.8/src/bioregistry/external/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/biolink.py` & `bioregistry-0.9.8/src/bioregistry/external/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/bioportal.py` & `bioregistry-0.9.8/src/bioregistry/external/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/cellosaurus.py` & `bioregistry-0.9.8/src/bioregistry/external/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/cheminf.py` & `bioregistry-0.9.8/src/bioregistry/external/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/cropoct.py` & `bioregistry-0.9.8/src/bioregistry/external/cropoct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/edam.py` & `bioregistry-0.9.8/src/bioregistry/external/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/fairsharing.py` & `bioregistry-0.9.8/src/bioregistry/external/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/go.py` & `bioregistry-0.9.8/src/bioregistry/external/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/hl7/OID_Report.csv` & `bioregistry-0.9.8/src/bioregistry/external/hl7/OID_Report.csv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/hl7/__init__.py` & `bioregistry-0.9.8/src/bioregistry/external/hl7/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/miriam.py` & `bioregistry-0.9.8/src/bioregistry/external/miriam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/n2t.py` & `bioregistry-0.9.8/src/bioregistry/external/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/ncbi.py` & `bioregistry-0.9.8/src/bioregistry/external/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/obofoundry.py` & `bioregistry-0.9.8/src/bioregistry/external/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/ols.py` & `bioregistry-0.9.8/src/bioregistry/external/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/ontobee.py` & `bioregistry-0.9.8/src/bioregistry/external/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/prefixcommons.py` & `bioregistry-0.9.8/src/bioregistry/external/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/re3data.py` & `bioregistry-0.9.8/src/bioregistry/external/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/uniprot.py` & `bioregistry-0.9.8/src/bioregistry/external/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/external/wikidata.py` & `bioregistry-0.9.8/src/bioregistry/external/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/gh/github_client.py` & `bioregistry-0.9.8/src/bioregistry/gh/github_client.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/gh/new_prefix.py` & `bioregistry-0.9.8/src/bioregistry/gh/new_prefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/health/check_homepages.py` & `bioregistry-0.9.8/src/bioregistry/health/check_homepages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/health/check_providers.py` & `bioregistry-0.9.8/src/bioregistry/health/check_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/health/cli.py` & `bioregistry-0.9.8/src/bioregistry/health/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/license_standardizer.py` & `bioregistry-0.9.8/src/bioregistry/license_standardizer.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/lint.py` & `bioregistry-0.9.8/src/bioregistry/lint.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/metaresource_api.py` & `bioregistry-0.9.8/src/bioregistry/metaresource_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/pandas.py` & `bioregistry-0.9.8/src/bioregistry/pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/parse_iri.py` & `bioregistry-0.9.8/src/bioregistry/parse_iri.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/record_accumulator.py` & `bioregistry-0.9.8/src/bioregistry/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/resolve.py` & `bioregistry-0.9.8/src/bioregistry/resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/resolve_identifier.py` & `bioregistry-0.9.8/src/bioregistry/resolve_identifier.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/resource_manager.py` & `bioregistry-0.9.8/src/bioregistry/resource_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/schema/constants.py` & `bioregistry-0.9.8/src/bioregistry/schema/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/schema/schema.json` & `bioregistry-0.9.8/src/bioregistry/schema/schema.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/schema/struct.py` & `bioregistry-0.9.8/src/bioregistry/schema/struct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/schema/utils.py` & `bioregistry-0.9.8/src/bioregistry/schema/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/schema_utils.py` & `bioregistry-0.9.8/src/bioregistry/schema_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/summary.py` & `bioregistry-0.9.8/src/bioregistry/summary.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/upload_ndex.py` & `bioregistry-0.9.8/src/bioregistry/upload_ndex.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/uri_format.py` & `bioregistry-0.9.8/src/bioregistry/uri_format.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/utils.py` & `bioregistry-0.9.8/src/bioregistry/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry/version.py` & `bioregistry-0.9.8/src/bioregistry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.9.7"
+VERSION = "0.9.8"
 
 
 def get_git_hash() -> Optional[str]:
     """Get the bioregistry git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioregistry-0.9.7/src/bioregistry.egg-info/PKG-INFO` & `bioregistry-0.9.8/src/bioregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.7
+Version: 0.9.8
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.7 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.8 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.7/src/bioregistry.egg-info/SOURCES.txt` & `bioregistry-0.9.8/src/bioregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/src/bioregistry.egg-info/requires.txt` & `bioregistry-0.9.8/src/bioregistry.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_api.py` & `bioregistry-0.9.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_collections.py` & `bioregistry-0.9.8/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_contexts.py` & `bioregistry-0.9.8/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_data.py` & `bioregistry-0.9.8/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_duplicates.py` & `bioregistry-0.9.8/tests/test_duplicates.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_identifiers_org.py` & `bioregistry-0.9.8/tests/test_identifiers_org.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_indra.py` & `bioregistry-0.9.8/tests/test_indra.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_manager.py` & `bioregistry-0.9.8/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_metaregistry.py` & `bioregistry-0.9.8/tests/test_metaregistry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_ols.py` & `bioregistry-0.9.8/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_pandas.py` & `bioregistry-0.9.8/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_resolve.py` & `bioregistry-0.9.8/tests/test_resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_sparql.py` & `bioregistry-0.9.8/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_usages.py` & `bioregistry-0.9.8/tests/test_usages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_utils.py` & `bioregistry-0.9.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_web/test_api.py` & `bioregistry-0.9.8/tests/test_web/test_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.7/tests/test_web/test_ui.py` & `bioregistry-0.9.8/tests/test_web/test_ui.py`

 * *Files identical despite different names*

