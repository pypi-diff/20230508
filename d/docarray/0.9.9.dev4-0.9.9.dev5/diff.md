# Comparing `tmp/docarray-0.9.9.dev4.tar.gz` & `tmp/docarray-0.9.9.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docarray-0.9.9.dev4.tar", last modified: Mon Mar 14 17:39:26 2022, max compression
+gzip compressed data, was "docarray-0.9.9.dev5.tar", last modified: Mon Mar 14 17:42:23 2022, max compression
```

## Comparing `docarray-0.9.9.dev4.tar` & `docarray-0.9.9.dev5.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/
--rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18803 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14157 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.412557 docarray-0.9.9.dev4/docarray/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.416557 docarray-0.9.9.dev4/docarray/array/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/annlite.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/chunk.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/document.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/match.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.416557 docarray-0.9.9.dev4/docarray/array/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/delitem.py
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/embed.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/empty.py
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8826 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/find.py
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/getattr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/getitem.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/group.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/mixins/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13088 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/binary.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     8495 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/from_gen.py
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/io/pushpull.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/match.py
--rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/parallel.py
--rw-r--r--   0 runner    (1001) docker     (121)    15539 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/post.py
--rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     8570 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/setitem.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     6380 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/mixins/traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/queryset/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/queryset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8376 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/queryset/lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/queryset/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/annlite/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/find.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/annlite/seqlike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/base/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)    10426 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/base/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/base/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/base/seqlike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/memory/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/memory/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     7598 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/memory/find.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/memory/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/memory/seqlike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/qdrant/
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/find.py
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/qdrant/seqlike.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/sqlite/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/sqlite/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/sqlite/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/sqlite/seqlike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.420558 docarray-0.9.9.dev4/docarray/array/storage/weaviate/
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12118 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/weaviate/backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/weaviate/find.py
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/weaviate/getsetdel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/storage/weaviate/seqlike.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/array/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/document/
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3906 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11984 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/document/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5382 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/_property.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/blob.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/featurehash.py
--rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    16749 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/porting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/property.py
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/sugar.py
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/text.py
--rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/mixins/video.py
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/pydantic_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/document/strawberry_type.py
--rw-r--r--   0 runner    (1001) docker     (121)    12686 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/math/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/math/distance/
--rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/distance/numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/distance/paddle.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/distance/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/distance/torch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5862 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/math/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/proto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28365 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/proto/docarray_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/proto/io/
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/proto/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/proto/io/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.424558 docarray-0.9.9.dev4/docarray/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/resources/ci-vendors.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/docarray/resources/embedding-projector/
--rw-r--r--   0 runner    (1001) docker     (121)   494360 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/resources/embedding-projector/index.html.gz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/docarray/score/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/score/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/score/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/docarray/score/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/score/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/score/mixins/property.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/score/mixins/representer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/docarray/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:39:26.416557 docarray-0.9.9.dev4/docarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18803 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-14 17:39:26.000000 docarray-0.9.9.dev4/docarray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 17:39:26.428558 docarray-0.9.9.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-03-14 17:39:19.000000 docarray-0.9.9.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.731224 docarray-0.9.9.dev5/
+-rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    18803 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14157 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.715224 docarray-0.9.9.dev5/docarray/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.715224 docarray-0.9.9.dev5/docarray/array/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/annlite.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/document.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/match.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.719224 docarray-0.9.9.dev5/docarray/array/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/delitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/embed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/empty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8826 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/find.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/group.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.719224 docarray-0.9.9.dev5/docarray/array/mixins/io/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13088 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/binary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4020 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8495 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/from_gen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/io/pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/match.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9831 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15539 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2379 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/post.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1163 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4093 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8570 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/setitem.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6380 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/mixins/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.719224 docarray-0.9.9.dev5/docarray/array/queryset/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/queryset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8376 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/queryset/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/queryset/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.719224 docarray-0.9.9.dev5/docarray/array/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.719224 docarray-0.9.9.dev5/docarray/array/storage/annlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2968 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/find.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/annlite/seqlike.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/array/storage/base/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/base/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10426 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/base/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/base/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/base/seqlike.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/array/storage/memory/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/memory/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7598 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/memory/find.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/memory/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/memory/seqlike.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/array/storage/qdrant/
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/find.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/qdrant/seqlike.py
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/array/storage/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4619 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/sqlite/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/sqlite/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/sqlite/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2812 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/sqlite/seqlike.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/array/storage/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12118 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/weaviate/backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3154 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/weaviate/find.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/weaviate/getsetdel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2996 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/storage/weaviate/seqlike.py
+-rw-r--r--   0 runner    (1001) docker     (121)      671 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/array/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.723224 docarray-0.9.9.dev5/docarray/document/
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3906 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11984 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/document/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5382 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/_property.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/blob.py
+-rw-r--r--   0 runner    (1001) docker     (121)      831 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/dump.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/featurehash.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16749 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/porting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/property.py
+-rw-r--r--   0 runner    (1001) docker     (121)      758 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/sugar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2397 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/mixins/video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/pydantic_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/document/strawberry_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12686 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/math/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/math/distance/
+-rw-r--r--   0 runner    (1001) docker     (121)     3947 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/distance/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/distance/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/distance/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/distance/torch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5600 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3205 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5862 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/math/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28365 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/proto/docarray_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/proto/io/
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/proto/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5158 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/proto/io/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/resources/ci-vendors.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/resources/embedding-projector/
+-rw-r--r--   0 runner    (1001) docker     (121)   494360 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/resources/embedding-projector/index.html.gz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/score/
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/score/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/score/data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.727224 docarray-0.9.9.dev5/docarray/score/mixins/
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/score/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/score/mixins/property.py
+-rw-r--r--   0 runner    (1001) docker     (121)      174 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/score/mixins/representer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/docarray/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:42:23.715224 docarray-0.9.9.dev5/docarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    18803 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4555 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-14 17:42:23.000000 docarray-0.9.9.dev5/docarray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 17:42:23.731224 docarray-0.9.9.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4101 2022-03-14 17:42:17.000000 docarray-0.9.9.dev5/setup.py
```

### Comparing `docarray-0.9.9.dev4/LICENSE` & `docarray-0.9.9.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/PKG-INFO` & `docarray-0.9.9.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docarray
-Version: 0.9.9.dev4
+Version: 0.9.9.dev5
 Summary: The data structure for unstructured data
 Home-page: https://github.com/jina-ai/docarray
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/docarray/tags
 Project-URL: Documentation, https://docarray.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docarray Version: 0.9.9.dev4 Summary: The data
+Metadata-Version: 2.1 Name: docarray Version: 0.9.9.dev5 Summary: The data
 structure for unstructured data Home-page: https://github.com/jina-ai/docarray
 Author: Jina AI Author-email: hello@jina.ai License: Apache 2.0 Download-URL:
 https://github.com/jina-ai/docarray/tags Project-URL: Documentation, https://
 docarray.jina.ai Project-URL: Source, https://github.com/jina-ai/docarray/
 Project-URL: Tracker, https://github.com/jina-ai/docarray/issues Description:
           [DocArray logo: The data structure for unstructured data]
                    The data structure for unstructured data
```

### Comparing `docarray-0.9.9.dev4/README.md` & `docarray-0.9.9.dev5/README.md`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/chunk.py` & `docarray-0.9.9.dev5/docarray/array/chunk.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/document.py` & `docarray-0.9.9.dev5/docarray/array/document.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/match.py` & `docarray-0.9.9.dev5/docarray/array/match.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/__init__.py` & `docarray-0.9.9.dev5/docarray/array/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/content.py` & `docarray-0.9.9.dev5/docarray/array/mixins/content.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/delitem.py` & `docarray-0.9.9.dev5/docarray/array/mixins/delitem.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/embed.py` & `docarray-0.9.9.dev5/docarray/array/mixins/embed.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/empty.py` & `docarray-0.9.9.dev5/docarray/array/mixins/empty.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/evaluation.py` & `docarray-0.9.9.dev5/docarray/array/mixins/evaluation.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/find.py` & `docarray-0.9.9.dev5/docarray/array/mixins/find.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/getattr.py` & `docarray-0.9.9.dev5/docarray/array/mixins/getattr.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/getitem.py` & `docarray-0.9.9.dev5/docarray/array/mixins/getitem.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/group.py` & `docarray-0.9.9.dev5/docarray/array/mixins/group.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/binary.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/binary.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/common.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/common.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/csv.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/csv.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/dataframe.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/from_gen.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/from_gen.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/json.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/json.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/io/pushpull.py` & `docarray-0.9.9.dev5/docarray/array/mixins/io/pushpull.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/match.py` & `docarray-0.9.9.dev5/docarray/array/mixins/match.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/parallel.py` & `docarray-0.9.9.dev5/docarray/array/mixins/parallel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/plot.py` & `docarray-0.9.9.dev5/docarray/array/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/post.py` & `docarray-0.9.9.dev5/docarray/array/mixins/post.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/pydantic.py` & `docarray-0.9.9.dev5/docarray/array/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/reduce.py` & `docarray-0.9.9.dev5/docarray/array/mixins/reduce.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/sample.py` & `docarray-0.9.9.dev5/docarray/array/mixins/sample.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/setitem.py` & `docarray-0.9.9.dev5/docarray/array/mixins/setitem.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/strawberry.py` & `docarray-0.9.9.dev5/docarray/array/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/text.py` & `docarray-0.9.9.dev5/docarray/array/mixins/text.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/mixins/traverse.py` & `docarray-0.9.9.dev5/docarray/array/mixins/traverse.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/qdrant.py` & `docarray-0.9.9.dev5/docarray/array/qdrant.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/queryset/lookup.py` & `docarray-0.9.9.dev5/docarray/array/queryset/lookup.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/queryset/parser.py` & `docarray-0.9.9.dev5/docarray/array/queryset/parser.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/annlite/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/annlite/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/annlite/find.py` & `docarray-0.9.9.dev5/docarray/array/storage/annlite/find.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/annlite/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/annlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/annlite/helper.py` & `docarray-0.9.9.dev5/docarray/array/storage/annlite/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/annlite/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/annlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/base/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/base/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/base/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/base/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/base/helper.py` & `docarray-0.9.9.dev5/docarray/array/storage/base/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/base/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/base/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/memory/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/memory/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/memory/find.py` & `docarray-0.9.9.dev5/docarray/array/storage/memory/find.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/memory/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/memory/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/memory/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/memory/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/qdrant/__init__.py` & `docarray-0.9.9.dev5/docarray/array/storage/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/qdrant/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/qdrant/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/qdrant/find.py` & `docarray-0.9.9.dev5/docarray/array/storage/qdrant/find.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/qdrant/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/qdrant/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/qdrant/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/qdrant/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/sqlite/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/sqlite/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/sqlite/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/sqlite/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/sqlite/helper.py` & `docarray-0.9.9.dev5/docarray/array/storage/sqlite/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/sqlite/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/sqlite/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/weaviate/backend.py` & `docarray-0.9.9.dev5/docarray/array/storage/weaviate/backend.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/weaviate/find.py` & `docarray-0.9.9.dev5/docarray/array/storage/weaviate/find.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/weaviate/getsetdel.py` & `docarray-0.9.9.dev5/docarray/array/storage/weaviate/getsetdel.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/storage/weaviate/seqlike.py` & `docarray-0.9.9.dev5/docarray/array/storage/weaviate/seqlike.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/array/weaviate.py` & `docarray-0.9.9.dev5/docarray/array/weaviate.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/base.py` & `docarray-0.9.9.dev5/docarray/base.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/__init__.py` & `docarray-0.9.9.dev5/docarray/document/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/data.py` & `docarray-0.9.9.dev5/docarray/document/data.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/generators.py` & `docarray-0.9.9.dev5/docarray/document/generators.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/__init__.py` & `docarray-0.9.9.dev5/docarray/document/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/_property.py` & `docarray-0.9.9.dev5/docarray/document/mixins/_property.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/attribute.py` & `docarray-0.9.9.dev5/docarray/document/mixins/attribute.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/audio.py` & `docarray-0.9.9.dev5/docarray/document/mixins/audio.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/blob.py` & `docarray-0.9.9.dev5/docarray/document/mixins/blob.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/content.py` & `docarray-0.9.9.dev5/docarray/document/mixins/content.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/convert.py` & `docarray-0.9.9.dev5/docarray/document/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/dump.py` & `docarray-0.9.9.dev5/docarray/document/mixins/dump.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/featurehash.py` & `docarray-0.9.9.dev5/docarray/document/mixins/featurehash.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/helper.py` & `docarray-0.9.9.dev5/docarray/document/mixins/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/image.py` & `docarray-0.9.9.dev5/docarray/document/mixins/image.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/mesh.py` & `docarray-0.9.9.dev5/docarray/document/mixins/mesh.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/plot.py` & `docarray-0.9.9.dev5/docarray/document/mixins/plot.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/porting.py` & `docarray-0.9.9.dev5/docarray/document/mixins/porting.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/property.py` & `docarray-0.9.9.dev5/docarray/document/mixins/property.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/protobuf.py` & `docarray-0.9.9.dev5/docarray/document/mixins/protobuf.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/pydantic.py` & `docarray-0.9.9.dev5/docarray/document/mixins/pydantic.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/strawberry.py` & `docarray-0.9.9.dev5/docarray/document/mixins/strawberry.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/sugar.py` & `docarray-0.9.9.dev5/docarray/document/mixins/sugar.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/text.py` & `docarray-0.9.9.dev5/docarray/document/mixins/text.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/mixins/video.py` & `docarray-0.9.9.dev5/docarray/document/mixins/video.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/pydantic_model.py` & `docarray-0.9.9.dev5/docarray/document/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/document/strawberry_type.py` & `docarray-0.9.9.dev5/docarray/document/strawberry_type.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/helper.py` & `docarray-0.9.9.dev5/docarray/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/distance/__init__.py` & `docarray-0.9.9.dev5/docarray/math/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/distance/numpy.py` & `docarray-0.9.9.dev5/docarray/math/distance/numpy.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/distance/paddle.py` & `docarray-0.9.9.dev5/docarray/math/distance/paddle.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/distance/tensorflow.py` & `docarray-0.9.9.dev5/docarray/math/distance/tensorflow.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/distance/torch.py` & `docarray-0.9.9.dev5/docarray/math/distance/torch.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/evaluation.py` & `docarray-0.9.9.dev5/docarray/math/evaluation.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/helper.py` & `docarray-0.9.9.dev5/docarray/math/helper.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/math/ndarray.py` & `docarray-0.9.9.dev5/docarray/math/ndarray.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/proto/docarray_pb2.py` & `docarray-0.9.9.dev5/docarray/proto/docarray_pb2.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/proto/io/__init__.py` & `docarray-0.9.9.dev5/docarray/proto/io/__init__.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/proto/io/ndarray.py` & `docarray-0.9.9.dev5/docarray/proto/io/ndarray.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/resources/ci-vendors.json` & `docarray-0.9.9.dev5/docarray/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/resources/embedding-projector/index.html.gz` & `docarray-0.9.9.dev5/docarray/resources/embedding-projector/index.html.gz`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/score/data.py` & `docarray-0.9.9.dev5/docarray/score/data.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/score/mixins/property.py` & `docarray-0.9.9.dev5/docarray/score/mixins/property.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray/types.py` & `docarray-0.9.9.dev5/docarray/types.py`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray.egg-info/PKG-INFO` & `docarray-0.9.9.dev5/docarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docarray
-Version: 0.9.9.dev4
+Version: 0.9.9.dev5
 Summary: The data structure for unstructured data
 Home-page: https://github.com/jina-ai/docarray
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/docarray/tags
 Project-URL: Documentation, https://docarray.jina.ai
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docarray Version: 0.9.9.dev4 Summary: The data
+Metadata-Version: 2.1 Name: docarray Version: 0.9.9.dev5 Summary: The data
 structure for unstructured data Home-page: https://github.com/jina-ai/docarray
 Author: Jina AI Author-email: hello@jina.ai License: Apache 2.0 Download-URL:
 https://github.com/jina-ai/docarray/tags Project-URL: Documentation, https://
 docarray.jina.ai Project-URL: Source, https://github.com/jina-ai/docarray/
 Project-URL: Tracker, https://github.com/jina-ai/docarray/issues Description:
           [DocArray logo: The data structure for unstructured data]
                    The data structure for unstructured data
```

### Comparing `docarray-0.9.9.dev4/docarray.egg-info/SOURCES.txt` & `docarray-0.9.9.dev5/docarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/docarray.egg-info/requires.txt` & `docarray-0.9.9.dev5/docarray.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `docarray-0.9.9.dev4/setup.py` & `docarray-0.9.9.dev5/setup.py`

 * *Files identical despite different names*

