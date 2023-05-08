# Comparing `tmp/types-graphene-0.21.tar.gz` & `tmp/types-graphene-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-graphene-0.21.tar", last modified: Wed May  3 09:27:33 2023, max compression
+gzip compressed data, was "types-graphene-0.22.tar", last modified: Mon May  8 08:41:54 2023, max compression
```

## Comparing `types-graphene-0.21.tar` & `types-graphene-0.22.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.517250 types-graphene-0.21/
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1074 2023-04-10 02:39:32.000000 types-graphene-0.21/LICENSE
--rw-r--r--   0 dongzoolee   (501) staff       (20)      424 2023-05-03 09:27:33.517027 types-graphene-0.21/PKG-INFO
--rw-r--r--   0 dongzoolee   (501) staff       (20)     3239 2023-04-10 02:39:32.000000 types-graphene-0.21/README.md
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.489594 types-graphene-0.21/graphene-stubs/
--rw-r--r--   0 dongzoolee   (501) staff       (20)      963 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/__init__.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.490941 types-graphene-0.21/graphene-stubs/pyutils/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/pyutils/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      170 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/pyutils/compat.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      292 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/pyutils/init_subclass.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     2437 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/pyutils/signature.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      350 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/pyutils/version.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.492020 types-graphene-0.21/graphene-stubs/relay/
--rw-r--r--   0 dongzoolee   (501) staff       (20)      239 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1546 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/connection.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      707 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/mutation.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1906 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/node.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.493447 types-graphene-0.21/graphene-stubs/relay/tests/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      902 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_connection.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     2307 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_connection_query.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      764 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_global_id.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     2197 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_mutation.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1357 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_node.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1366 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/relay/tests/test_node_custom.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.493687 types-graphene-0.21/graphene-stubs/test/
--rw-r--r--   0 dongzoolee   (501) staff       (20)      534 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/test/__init__.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.493897 types-graphene-0.21/graphene-stubs/tests/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/__init__.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.495334 types-graphene-0.21/graphene-stubs/tests/issues/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      550 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_313.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      268 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_356.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1530 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_425.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      225 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_490.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      505 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_720.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       30 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/tests/issues/test_956.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.501890 types-graphene-0.21/graphene-stubs/types/
--rw-r--r--   0 dongzoolee   (501) staff       (20)      968 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      286 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/abstracttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      779 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/argument.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      777 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/base.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       99 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/context.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      824 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/datetime.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      299 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/decimal.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      757 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/definitions.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      356 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/dynamic.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1382 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/enum.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1173 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/field.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      357 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/generic.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      718 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/inputfield.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1000 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/inputobjecttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      685 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/interface.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      304 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/json.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      248 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/mountedtype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1197 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/mutation.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      865 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/objecttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      493 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/resolver.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1493 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/scalars.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1039 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/schema.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      518 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/structures.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.508450 types-graphene-0.21/graphene-stubs/types/tests/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      503 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_abstracttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      613 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_argument.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      445 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_base.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1227 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_datetime.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      421 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_decimal.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1863 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_definition.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      297 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_dynamic.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1037 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_enum.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      934 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_field.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      417 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_generic.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      341 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_inputfield.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1035 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_inputobjecttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      686 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_interface.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      368 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_json.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      293 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_mountedtype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      760 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_mutation.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     2050 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_objecttype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1617 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_query.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      675 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_resolver.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       71 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_scalar.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      281 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_scalars_serialization.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      480 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_schema.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      894 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_structures.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      881 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_typemap.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      441 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_union.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      356 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/test_uuid.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       40 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/tests/utils.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)     2547 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/typemap.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      653 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/union.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      516 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/unmountedtype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      426 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/utils.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      293 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/types/uuid.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.512264 types-graphene-0.21/graphene-stubs/utils/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      279 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/annotate.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      236 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/crunch.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      129 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/deduplicator.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      139 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/deprecated.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       77 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/get_unbound_function.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      219 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/module_loading.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      488 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/orderedtype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       97 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/props.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      118 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/resolve_only_args.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      166 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/str_converters.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      397 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/subclass_with_meta.pyi
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.515112 types-graphene-0.21/graphene-stubs/utils/tests/
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/__init__.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      362 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_annotate.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      141 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_crunch.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      492 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_deduplicator.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      461 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_deprecated.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      365 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_module_loading.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      274 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_orderedtype.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      187 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_resolve_only_args.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_resolver_from_annotations.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      218 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_str_converters.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      102 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/tests/test_trim_docstring.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)      182 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/thenables.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       90 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/thenables_asyncio.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)       76 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene-stubs/utils/trim_docstring.pyi
--rw-r--r--   0 dongzoolee   (501) staff       (20)    34064 2023-04-10 13:17:28.000000 types-graphene-0.21/graphene_plugin.py
--rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.21/graphene_typing.py
--rw-r--r--   0 dongzoolee   (501) staff       (20)       38 2023-05-03 09:27:33.517300 types-graphene-0.21/setup.cfg
--rw-r--r--   0 dongzoolee   (501) staff       (20)     1218 2023-05-03 09:26:43.000000 types-graphene-0.21/setup.py
-drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-03 09:27:33.516757 types-graphene-0.21/types_graphene.egg-info/
--rw-r--r--   0 dongzoolee   (501) staff       (20)      424 2023-05-03 09:27:33.000000 types-graphene-0.21/types_graphene.egg-info/PKG-INFO
--rw-r--r--   0 dongzoolee   (501) staff       (20)     4584 2023-05-03 09:27:33.000000 types-graphene-0.21/types_graphene.egg-info/SOURCES.txt
--rw-r--r--   0 dongzoolee   (501) staff       (20)        1 2023-05-03 09:27:33.000000 types-graphene-0.21/types_graphene.egg-info/dependency_links.txt
--rw-r--r--   0 dongzoolee   (501) staff       (20)       37 2023-05-03 09:27:33.000000 types-graphene-0.21/types_graphene.egg-info/requires.txt
--rw-r--r--   0 dongzoolee   (501) staff       (20)       47 2023-05-03 09:27:33.000000 types-graphene-0.21/types_graphene.egg-info/top_level.txt
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:54.006263 types-graphene-0.22/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1074 2023-04-10 02:39:32.000000 types-graphene-0.22/LICENSE
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      424 2023-05-08 08:41:54.006117 types-graphene-0.22/PKG-INFO
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     3239 2023-04-10 02:39:32.000000 types-graphene-0.22/README.md
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.986391 types-graphene-0.22/graphene-stubs/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      963 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/__init__.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.987624 types-graphene-0.22/graphene-stubs/pyutils/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/pyutils/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      170 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/pyutils/compat.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      292 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/pyutils/init_subclass.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     2437 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/pyutils/signature.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      350 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/pyutils/version.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.988574 types-graphene-0.22/graphene-stubs/relay/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      239 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1546 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/connection.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      707 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/mutation.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1906 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/node.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.989958 types-graphene-0.22/graphene-stubs/relay/tests/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      902 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_connection.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     2307 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_connection_query.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      764 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_global_id.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     2197 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_mutation.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1357 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_node.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1366 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/relay/tests/test_node_custom.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.990168 types-graphene-0.22/graphene-stubs/test/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      534 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/test/__init__.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.990378 types-graphene-0.22/graphene-stubs/tests/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/__init__.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.991535 types-graphene-0.22/graphene-stubs/tests/issues/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      550 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_313.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      268 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_356.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1530 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_425.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      225 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_490.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      505 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_720.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       30 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/tests/issues/test_956.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:53.996645 types-graphene-0.22/graphene-stubs/types/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      968 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      286 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/abstracttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      779 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/argument.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      777 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/base.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       99 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/context.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      824 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/datetime.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      299 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/decimal.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      757 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/definitions.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      356 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/dynamic.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1382 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/enum.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1173 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/field.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      357 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/generic.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      718 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/inputfield.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1000 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/inputobjecttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      685 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/interface.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      304 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/json.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      248 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/mountedtype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1197 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/mutation.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      865 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/objecttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      493 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/resolver.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1548 2023-05-08 08:41:29.000000 types-graphene-0.22/graphene-stubs/types/scalars.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1039 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/schema.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      518 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/structures.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:54.001022 types-graphene-0.22/graphene-stubs/types/tests/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      503 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_abstracttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      613 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_argument.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      445 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_base.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1227 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_datetime.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      421 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_decimal.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1863 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_definition.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      297 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_dynamic.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1037 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_enum.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      934 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_field.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      417 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_generic.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      341 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_inputfield.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1035 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_inputobjecttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      686 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_interface.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      368 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_json.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      293 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_mountedtype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      760 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_mutation.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     2050 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_objecttype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1617 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_query.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      675 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_resolver.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       71 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_scalar.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      281 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_scalars_serialization.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      480 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_schema.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      894 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_structures.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      881 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_typemap.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      441 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_union.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      356 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/test_uuid.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       40 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/tests/utils.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     2547 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/typemap.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      653 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/union.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      516 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/unmountedtype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      426 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/utils.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      293 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/types/uuid.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:54.003369 types-graphene-0.22/graphene-stubs/utils/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      279 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/annotate.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      236 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/crunch.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      129 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/deduplicator.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      139 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/deprecated.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       77 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/get_unbound_function.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      219 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/module_loading.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      488 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/orderedtype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       97 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/props.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      118 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/resolve_only_args.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      166 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/str_converters.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      397 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/subclass_with_meta.pyi
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:54.005240 types-graphene-0.22/graphene-stubs/utils/tests/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/__init__.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      362 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_annotate.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      141 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_crunch.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      492 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_deduplicator.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      461 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_deprecated.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      365 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_module_loading.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      274 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_orderedtype.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      187 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_resolve_only_args.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_resolver_from_annotations.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      218 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_str_converters.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      102 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/tests/test_trim_docstring.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      182 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/thenables.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       90 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/thenables_asyncio.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       76 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene-stubs/utils/trim_docstring.pyi
+-rw-r--r--   0 dongzoolee   (501) staff       (20)    34064 2023-04-10 13:17:28.000000 types-graphene-0.22/graphene_plugin.py
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        0 2023-04-10 02:39:32.000000 types-graphene-0.22/graphene_typing.py
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       38 2023-05-08 08:41:54.006305 types-graphene-0.22/setup.cfg
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     1218 2023-05-08 08:41:50.000000 types-graphene-0.22/setup.py
+drwxr-xr-x   0 dongzoolee   (501) staff       (20)        0 2023-05-08 08:41:54.005916 types-graphene-0.22/types_graphene.egg-info/
+-rw-r--r--   0 dongzoolee   (501) staff       (20)      424 2023-05-08 08:41:53.000000 types-graphene-0.22/types_graphene.egg-info/PKG-INFO
+-rw-r--r--   0 dongzoolee   (501) staff       (20)     4584 2023-05-08 08:41:53.000000 types-graphene-0.22/types_graphene.egg-info/SOURCES.txt
+-rw-r--r--   0 dongzoolee   (501) staff       (20)        1 2023-05-08 08:41:53.000000 types-graphene-0.22/types_graphene.egg-info/dependency_links.txt
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       37 2023-05-08 08:41:53.000000 types-graphene-0.22/types_graphene.egg-info/requires.txt
+-rw-r--r--   0 dongzoolee   (501) staff       (20)       47 2023-05-08 08:41:53.000000 types-graphene-0.22/types_graphene.egg-info/top_level.txt
```

### Comparing `types-graphene-0.21/LICENSE` & `types-graphene-0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/README.md` & `types-graphene-0.22/README.md`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/__init__.pyi` & `types-graphene-0.22/graphene-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/pyutils/signature.pyi` & `types-graphene-0.22/graphene-stubs/pyutils/signature.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/connection.pyi` & `types-graphene-0.22/graphene-stubs/relay/connection.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/mutation.pyi` & `types-graphene-0.22/graphene-stubs/relay/mutation.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/node.pyi` & `types-graphene-0.22/graphene-stubs/relay/node.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_connection.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_connection_query.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_connection_query.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_global_id.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_global_id.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_mutation.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_mutation.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_node.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_node.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/relay/tests/test_node_custom.pyi` & `types-graphene-0.22/graphene-stubs/relay/tests/test_node_custom.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/test/__init__.pyi` & `types-graphene-0.22/graphene-stubs/test/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/tests/issues/test_313.pyi` & `types-graphene-0.22/graphene-stubs/tests/issues/test_313.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/tests/issues/test_425.pyi` & `types-graphene-0.22/graphene-stubs/tests/issues/test_425.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/__init__.pyi` & `types-graphene-0.22/graphene-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/argument.pyi` & `types-graphene-0.22/graphene-stubs/types/argument.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/base.pyi` & `types-graphene-0.22/graphene-stubs/types/base.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/datetime.pyi` & `types-graphene-0.22/graphene-stubs/types/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/definitions.pyi` & `types-graphene-0.22/graphene-stubs/types/definitions.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/enum.pyi` & `types-graphene-0.22/graphene-stubs/types/enum.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/field.pyi` & `types-graphene-0.22/graphene-stubs/types/field.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/inputfield.pyi` & `types-graphene-0.22/graphene-stubs/types/inputfield.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/inputobjecttype.pyi` & `types-graphene-0.22/graphene-stubs/types/inputobjecttype.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/interface.pyi` & `types-graphene-0.22/graphene-stubs/types/interface.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/mutation.pyi` & `types-graphene-0.22/graphene-stubs/types/mutation.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/objecttype.pyi` & `types-graphene-0.22/graphene-stubs/types/objecttype.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/scalars.pyi` & `types-graphene-0.22/graphene-stubs/types/scalars.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
     @staticmethod
     def parse_literal(ast: Any) -> Any:
         ...
 
 
 class String(Scalar):
+    @overload
+    def __new__(cls, *args) -> str: ...
+
     @staticmethod
     def coerce_string(value: Any) -> str:
         ...
 
     serialize = coerce_string
     parse_value = coerce_string
```

### Comparing `types-graphene-0.21/graphene-stubs/types/schema.pyi` & `types-graphene-0.22/graphene-stubs/types/schema.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/structures.pyi` & `types-graphene-0.22/graphene-stubs/types/structures.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_argument.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_argument.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_datetime.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_definition.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_definition.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_enum.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_enum.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_field.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_field.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_inputobjecttype.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_inputobjecttype.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_interface.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_interface.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_mutation.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_mutation.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_objecttype.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_objecttype.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_query.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_query.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_resolver.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_resolver.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_structures.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_structures.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/tests/test_typemap.pyi` & `types-graphene-0.22/graphene-stubs/types/tests/test_typemap.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/typemap.pyi` & `types-graphene-0.22/graphene-stubs/types/typemap.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/union.pyi` & `types-graphene-0.22/graphene-stubs/types/union.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene-stubs/types/unmountedtype.pyi` & `types-graphene-0.22/graphene-stubs/types/unmountedtype.pyi`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/graphene_plugin.py` & `types-graphene-0.22/graphene_plugin.py`

 * *Files identical despite different names*

### Comparing `types-graphene-0.21/setup.py` & `types-graphene-0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 result.append(file)
     print(result)
     return result
 
 
 setup(
     name="types-graphene",
-    version="0.21",
+    version="0.22",
     description=description,
     long_description=install_instructions,
     long_description_content_type="text/markdown",
     author="dongzoolee",
     author_email="me@leed.at",
     license="MIT License",
     url="https://github.com/dongzoolee/types-graphene",
```

### Comparing `types-graphene-0.21/types_graphene.egg-info/SOURCES.txt` & `types-graphene-0.22/types_graphene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

