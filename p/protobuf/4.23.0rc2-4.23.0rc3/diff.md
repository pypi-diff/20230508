# Comparing `tmp/protobuf-4.23.0rc2.tar.gz` & `tmp/protobuf-4.23.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/protobuf-4.23.0rc2.tar", last modified: Fri Apr 28 17:47:02 2023, max compression
+gzip compressed data, was "dist/protobuf-4.23.0rc3.tar", last modified: Fri May  5 16:35:44 2023, max compression
```

## Comparing `protobuf-4.23.0rc2.tar` & `protobuf-4.23.0rc3.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/
--r-xr-xr-x   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/MANIFEST.in
--rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/README.md
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/__init__.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1708 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/any_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2840 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/api_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/compiler/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/compiler/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3174 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    47968 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    61064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upb.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)   359010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    51014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8036 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6819 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)   136435 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    46876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/descriptor_pool.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/duration_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1362 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/empty_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1453 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/field_mask_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/internal/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1631 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15432 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/_parameterized.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6126 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/api_implementation.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5188 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/builder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/containers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    38796 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/decoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    28656 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/encoder.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8485 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/extension_dict.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/field_mask.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/message_listener.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    57025 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/python_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5439 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/testing_refleaks.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    16809 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/type_checkers.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/well_known_types.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8446 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/internal/wire_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    36297 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/json_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    14551 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8952 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/message_factory.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/proto_builder.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/pyext/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/pyext/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/pyext/cpp_message.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3772 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9146 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/service.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11417 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/service_reflection.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1475 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/source_context_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2722 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/struct_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/symbol_database.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4701 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/text_encoding.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)    64011 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/text_format.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/timestamp_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5132 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/type_pb2.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4486 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/unknown_fields.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/google/protobuf/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/util/__init__.py
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2727 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/google/protobuf/wrappers_pb2.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/
--rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/PKG-INFO
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6497 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/namespace_packages.txt
--rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/protobuf.egg-info/top_level.txt
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/python/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    15821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/convert.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/convert.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    69085 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    28410 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_containers.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_containers.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    22990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2222 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/descriptor_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9828 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/extension_dict.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1816 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/extension_dict.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    20520 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    71006 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11933 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/protobuf.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     9135 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/protobuf.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2928 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/python_api.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    31454 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/repeated.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3373 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/repeated.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/unknown_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1817 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/python/unknown_fields.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)       67 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/setup.cfg
--r-xr-xr-x   0 bazel     (1000) bazel     (1003)     3876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/setup.py
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/arena.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1795 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/array.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/base/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3670 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/descriptor_constants.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/log2.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3033 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/status.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2645 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2669 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/base/string_view.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/collections/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5012 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3672 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5080 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/array_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4755 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_gencode_util.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5900 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6037 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_sorter.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3986 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/map_sorter_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections/message_value.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1838 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/collections.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/extension_registry.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/hash/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25548 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7082 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4154 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/int_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/hash/str_table.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/json/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    44075 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2103 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    23909 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2883 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json_decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/json_encode.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/lex/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/atoi.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2256 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/atoi.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/round_trip.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/round_trip.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4061 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/strtod.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1872 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/strtod.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/unicode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3002 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/lex/unicode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1783 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/map.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/mem/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/alloc.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3564 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/alloc.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5352 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mem/arena_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/message/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3308 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    16666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12752 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/accessors_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10705 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/copy.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2614 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/copy.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3467 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/extension_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7003 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2831 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13430 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/promote.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4841 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/message/promote.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/mini_table/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4719 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6232 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3763 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/common_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    40569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8579 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12204 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4916 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/encode_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/enum_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2098 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_registry.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/extension_registry.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     6775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/field_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/file_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5149 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/message_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1818 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/sub_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2007 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table/types.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1807 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/mini_table.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1787 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/msg.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1798 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/msg_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/port/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/atomic.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/def.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2571 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/undef.inc
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2258 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/port/vsnprintf_compat.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2873 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2054 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11441 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_builder.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_builder_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    16058 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4588 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3349 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_pool_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_type.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3031 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/def_type.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2212 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/desc_state.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2402 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/desc_state_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    11150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2331 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3411 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2101 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2346 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_reserved_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5416 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/enum_value_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3751 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2263 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/extension_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    30643 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4217 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/field_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    12878 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3275 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2406 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/file_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8597 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4357 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25921 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     7420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2871 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3281 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2122 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/message_reserved_range_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4529 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2194 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/method_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8161 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3000 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2401 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/oneof_def_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4632 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2603 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2173 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/service_def_internal.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/
--rw-r--r--   0 bazel     (1000) bazel     (1003)   279249 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/descriptor.upb.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/reflection.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/status.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/string_view.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/text/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    13495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/text_encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1879 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/upb.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/util/
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10885 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/compare.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2866 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/compare.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    25065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/def_to_proto.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/def_to_proto.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    10836 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/required_fields.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4107 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/util/required_fields.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/upb/wire/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/common.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/common_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    49488 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     4418 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    51605 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_fast.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_fast.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5929 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/decode_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)    21305 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/encode.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3423 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/encode.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)    18408 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2721 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/reader.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     8847 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/reader.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     2367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/swap_internal.h
--rw-r--r--   0 bazel     (1000) bazel     (1003)     1906 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/upb/wire/types.h
-drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-04-28 17:47:02.000000 protobuf-4.23.0rc2/utf8_range/
--rw-r--r--   0 bazel     (1000) bazel     (1003)     3990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/naive.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5620 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/range2-neon.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)     5917 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/range2-sse.c
--rw-r--r--   0 bazel     (1000) bazel     (1003)      517 2000-01-01 00:00:00.000000 protobuf-4.23.0rc2/utf8_range/utf8_range.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/
+-r-xr-xr-x   0 bazel     (1000) bazel     (1003)       39 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/MANIFEST.in
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/README.md
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/__init__.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1708 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/any_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2840 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/api_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/protobuf/compiler/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/compiler/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3174 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/compiler/plugin_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    47968 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    61064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor.upb.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   359010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    51014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor.upbdefs.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8036 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor.upbdefs.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6819 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   136435 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    46876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/descriptor_pool.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/duration_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1362 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/empty_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1453 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/field_mask_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/protobuf/internal/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1631 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15432 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/_parameterized.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6126 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/api_implementation.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5188 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/builder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/containers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    38796 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/decoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    28656 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/encoder.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/enum_type_wrapper.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8485 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/extension_dict.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/field_mask.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/message_listener.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    57025 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/python_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5439 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/testing_refleaks.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16809 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/type_checkers.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20096 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/well_known_types.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8446 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/internal/wire_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    36297 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/json_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    14551 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8952 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/message_factory.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/proto_builder.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/protobuf/pyext/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/pyext/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/pyext/cpp_message.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3772 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9146 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/service.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11417 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/service_reflection.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1475 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/source_context_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2722 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/struct_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/symbol_database.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4701 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/text_encoding.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    64011 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/text_format.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1504 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/timestamp_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5132 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/type_pb2.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4486 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/unknown_fields.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/google/protobuf/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        0 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/util/__init__.py
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2727 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/google/protobuf/wrappers_pb2.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      777 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6497 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        1 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/namespace_packages.txt
+-rw-r--r--   0 bazel     (1000) bazel     (1003)        7 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/protobuf.egg-info/top_level.txt
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/python/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    15821 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/convert.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/convert.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    69085 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    28410 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor_containers.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor_containers.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    22990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2222 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/descriptor_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9828 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/extension_dict.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1816 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/extension_dict.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    20520 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3071 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    71006 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11933 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/protobuf.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     9135 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/protobuf.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2928 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/python_api.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    31454 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/repeated.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3373 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/repeated.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/unknown_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1817 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/python/unknown_fields.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)       67 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/setup.cfg
+-r-xr-xr-x   0 bazel     (1000) bazel     (1003)     3876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/setup.py
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1771 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/arena.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1795 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/array.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/base/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3670 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/base/descriptor_constants.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2078 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/base/log2.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3033 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/base/status.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2645 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/base/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2669 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/base/string_view.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/collections/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5012 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/array.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3672 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/array.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5080 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/array_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4755 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map_gencode_util.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5900 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6037 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map_sorter.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3986 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/map_sorter_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2376 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections/message_value.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1838 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/collections.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1799 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/extension_registry.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/hash/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25548 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/hash/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7082 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/hash/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4154 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/hash/int_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/hash/str_table.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/json/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    44075 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2103 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    23909 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2883 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json_decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/json_encode.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/lex/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2426 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/atoi.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2256 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/atoi.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/round_trip.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2328 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/round_trip.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4061 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/strtod.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1872 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/strtod.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2195 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/unicode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3002 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/lex/unicode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1783 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/map.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/mem/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1985 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mem/alloc.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3564 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mem/alloc.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13876 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mem/arena.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5352 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mem/arena.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mem/arena_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/message/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3308 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/accessors.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/accessors.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12752 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/accessors_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10705 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/copy.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2614 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/copy.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3467 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/extension_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5064 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7003 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2831 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13430 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/promote.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4841 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/message/promote.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/mini_table/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4719 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/common.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6232 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3763 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/common_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    40569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8579 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12204 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4916 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/encode_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3666 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/enum_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2098 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/extension_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/extension_registry.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4829 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/extension_registry.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     6775 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/field_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1989 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/file_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5149 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/message_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1818 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/sub_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2007 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table/types.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1807 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/mini_table.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1787 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/msg.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1798 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/msg_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/port/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/port/atomic.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10443 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/port/def.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2571 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/port/undef.inc
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2258 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/port/vsnprintf_compat.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/reflection/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2873 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2054 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11441 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_builder.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7014 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_builder_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    16058 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_pool.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4588 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_pool.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3349 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_pool_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_type.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3031 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/def_type.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2212 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/desc_state.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2402 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/desc_state_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    11150 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3562 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2331 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3411 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2101 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2346 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_reserved_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5416 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_value_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_value_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2422 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/enum_value_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3751 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/extension_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2244 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/extension_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2263 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/extension_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    30643 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/field_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4217 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/field_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/field_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    12878 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/file_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3275 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/file_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2406 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/file_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8597 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4357 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25921 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     7420 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2871 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3281 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_reserved_range.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2122 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_reserved_range.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2324 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/message_reserved_range_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4529 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/method_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2569 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/method_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2194 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/method_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8161 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/oneof_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3000 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/oneof_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2401 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/oneof_def_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4632 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/service_def.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2603 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/service_def.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2173 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/service_def_internal.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/reflection/stage0/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/reflection/stage0/google/
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/reflection/stage0/google/protobuf/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)   279249 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection/stage0/google/protobuf/descriptor.upb.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1813 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/reflection.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1780 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/status.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1810 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/string_view.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/text/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    13495 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/text/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2740 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/text/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1792 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/text_encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1879 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/upb.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/util/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10885 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/compare.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2866 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/compare.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    25065 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/def_to_proto.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/def_to_proto.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    10836 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/required_fields.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4107 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/util/required_fields.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/upb/wire/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1811 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/common.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2023 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/common_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    49488 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/decode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     4418 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/decode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    51605 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/decode_fast.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5245 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/decode_fast.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5929 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/decode_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    21305 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/encode.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3423 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/encode.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2010 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/eps_copy_input_stream.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)    18408 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/eps_copy_input_stream.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2721 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/reader.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     8847 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/reader.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     2367 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/swap_internal.h
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     1906 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/upb/wire/types.h
+drwxr-sr-x   0 bazel     (1000) bazel     (1003)        0 2023-05-05 16:35:44.000000 protobuf-4.23.0rc3/utf8_range/
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     3990 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/utf8_range/naive.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5620 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/utf8_range/range2-neon.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)     5917 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/utf8_range/range2-sse.c
+-rw-r--r--   0 bazel     (1000) bazel     (1003)      517 2000-01-01 00:00:00.000000 protobuf-4.23.0rc3/utf8_range/utf8_range.h
```

### Comparing `protobuf-4.23.0rc2/PKG-INFO` & `protobuf-4.23.0rc3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: protobuf
-Version: 4.23.0rc2
+Version: 4.23.0rc3
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-4.23.0rc2/README.md` & `protobuf-4.23.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/__init__.py` & `protobuf-4.23.0rc3/google/protobuf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 # Copyright 2007 Google Inc. All Rights Reserved.
 
-__version__ = '4.23.0rc2'
+__version__ = '4.23.0rc3'
```

### Comparing `protobuf-4.23.0rc2/google/protobuf/any_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/any_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/api_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/api_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/compiler/plugin_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/compiler/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor.py` & `protobuf-4.23.0rc3/google/protobuf/descriptor.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor.upb.c` & `protobuf-4.23.0rc3/google/protobuf/descriptor.upb.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor.upb.h` & `protobuf-4.23.0rc3/google/protobuf/descriptor.upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.c` & `protobuf-4.23.0rc3/google/protobuf/descriptor.upbdefs.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor.upbdefs.h` & `protobuf-4.23.0rc3/google/protobuf/descriptor.upbdefs.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor_database.py` & `protobuf-4.23.0rc3/google/protobuf/descriptor_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/descriptor_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/descriptor_pool.py` & `protobuf-4.23.0rc3/google/protobuf/descriptor_pool.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/duration_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/duration_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/empty_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/empty_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/field_mask_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/field_mask_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/__init__.py` & `protobuf-4.23.0rc3/google/protobuf/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/_parameterized.py` & `protobuf-4.23.0rc3/google/protobuf/internal/_parameterized.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/api_implementation.py` & `protobuf-4.23.0rc3/google/protobuf/internal/api_implementation.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/builder.py` & `protobuf-4.23.0rc3/google/protobuf/internal/builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/containers.py` & `protobuf-4.23.0rc3/google/protobuf/internal/containers.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/decoder.py` & `protobuf-4.23.0rc3/google/protobuf/internal/decoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/encoder.py` & `protobuf-4.23.0rc3/google/protobuf/internal/encoder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/enum_type_wrapper.py` & `protobuf-4.23.0rc3/google/protobuf/internal/enum_type_wrapper.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/extension_dict.py` & `protobuf-4.23.0rc3/google/protobuf/internal/extension_dict.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/field_mask.py` & `protobuf-4.23.0rc3/google/protobuf/internal/field_mask.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/message_listener.py` & `protobuf-4.23.0rc3/google/protobuf/internal/message_listener.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/python_message.py` & `protobuf-4.23.0rc3/google/protobuf/internal/python_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/testing_refleaks.py` & `protobuf-4.23.0rc3/google/protobuf/internal/testing_refleaks.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/type_checkers.py` & `protobuf-4.23.0rc3/google/protobuf/internal/type_checkers.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/well_known_types.py` & `protobuf-4.23.0rc3/google/protobuf/internal/well_known_types.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/internal/wire_format.py` & `protobuf-4.23.0rc3/google/protobuf/internal/wire_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/json_format.py` & `protobuf-4.23.0rc3/google/protobuf/json_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/message.py` & `protobuf-4.23.0rc3/google/protobuf/message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/message_factory.py` & `protobuf-4.23.0rc3/google/protobuf/message_factory.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/proto_builder.py` & `protobuf-4.23.0rc3/google/protobuf/proto_builder.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/pyext/cpp_message.py` & `protobuf-4.23.0rc3/google/protobuf/pyext/cpp_message.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/reflection.py` & `protobuf-4.23.0rc3/google/protobuf/reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/service.py` & `protobuf-4.23.0rc3/google/protobuf/service.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/service_reflection.py` & `protobuf-4.23.0rc3/google/protobuf/service_reflection.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/source_context_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/source_context_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/struct_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/symbol_database.py` & `protobuf-4.23.0rc3/google/protobuf/symbol_database.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/text_encoding.py` & `protobuf-4.23.0rc3/google/protobuf/text_encoding.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/text_format.py` & `protobuf-4.23.0rc3/google/protobuf/text_format.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/timestamp_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/timestamp_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/type_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/unknown_fields.py` & `protobuf-4.23.0rc3/google/protobuf/unknown_fields.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/google/protobuf/wrappers_pb2.py` & `protobuf-4.23.0rc3/google/protobuf/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/protobuf.egg-info/PKG-INFO` & `protobuf-4.23.0rc3/protobuf.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: protobuf
-Version: 4.23.0rc2
+Version: 4.23.0rc3
 Summary: Protocol Buffers
 Home-page: https://developers.google.com/protocol-buffers/
 Maintainer: protobuf@googlegroups.com
 Maintainer-email: protobuf@googlegroups.com
 License: BSD-3-Clause
 Download-URL: https://github.com/protocolbuffers/protobuf/releases
 Project-URL: Source, https://github.com/protocolbuffers/protobuf
```

### Comparing `protobuf-4.23.0rc2/protobuf.egg-info/SOURCES.txt` & `protobuf-4.23.0rc3/protobuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/convert.c` & `protobuf-4.23.0rc3/python/convert.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/convert.h` & `protobuf-4.23.0rc3/python/convert.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor.c` & `protobuf-4.23.0rc3/python/descriptor.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor.h` & `protobuf-4.23.0rc3/python/descriptor.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor_containers.c` & `protobuf-4.23.0rc3/python/descriptor_containers.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor_containers.h` & `protobuf-4.23.0rc3/python/descriptor_containers.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor_pool.c` & `protobuf-4.23.0rc3/python/descriptor_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/descriptor_pool.h` & `protobuf-4.23.0rc3/python/descriptor_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/extension_dict.c` & `protobuf-4.23.0rc3/python/extension_dict.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/extension_dict.h` & `protobuf-4.23.0rc3/python/extension_dict.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/map.c` & `protobuf-4.23.0rc3/python/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/map.h` & `protobuf-4.23.0rc3/python/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/message.c` & `protobuf-4.23.0rc3/python/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/message.h` & `protobuf-4.23.0rc3/python/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/protobuf.c` & `protobuf-4.23.0rc3/python/protobuf.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/protobuf.h` & `protobuf-4.23.0rc3/python/protobuf.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/python_api.h` & `protobuf-4.23.0rc3/python/python_api.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/repeated.c` & `protobuf-4.23.0rc3/python/repeated.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/repeated.h` & `protobuf-4.23.0rc3/python/repeated.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/unknown_fields.c` & `protobuf-4.23.0rc3/python/unknown_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/python/unknown_fields.h` & `protobuf-4.23.0rc3/python/unknown_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/setup.py` & `protobuf-4.23.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/alloc.h` & `protobuf-4.23.0rc3/upb/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/arena.h` & `protobuf-4.23.0rc3/upb/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/array.h` & `protobuf-4.23.0rc3/upb/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/base/descriptor_constants.h` & `protobuf-4.23.0rc3/upb/base/descriptor_constants.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/base/log2.h` & `protobuf-4.23.0rc3/upb/base/log2.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/base/status.c` & `protobuf-4.23.0rc3/upb/base/status.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/base/status.h` & `protobuf-4.23.0rc3/upb/base/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/base/string_view.h` & `protobuf-4.23.0rc3/upb/base/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/array.c` & `protobuf-4.23.0rc3/upb/collections/array.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/array.h` & `protobuf-4.23.0rc3/upb/collections/array.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/array_internal.h` & `protobuf-4.23.0rc3/upb/collections/array_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map.c` & `protobuf-4.23.0rc3/upb/collections/map.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map.h` & `protobuf-4.23.0rc3/upb/collections/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map_gencode_util.h` & `protobuf-4.23.0rc3/upb/collections/map_gencode_util.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map_internal.h` & `protobuf-4.23.0rc3/upb/collections/map_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map_sorter.c` & `protobuf-4.23.0rc3/upb/collections/map_sorter.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/map_sorter_internal.h` & `protobuf-4.23.0rc3/upb/collections/map_sorter_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections/message_value.h` & `protobuf-4.23.0rc3/upb/collections/message_value.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/collections.h` & `protobuf-4.23.0rc3/upb/collections.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/decode.h` & `protobuf-4.23.0rc3/upb/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/decode_fast.h` & `protobuf-4.23.0rc3/upb/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/def.h` & `protobuf-4.23.0rc3/upb/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/encode.h` & `protobuf-4.23.0rc3/upb/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/extension_registry.h` & `protobuf-4.23.0rc3/upb/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/hash/common.c` & `protobuf-4.23.0rc3/upb/hash/common.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/hash/common.h` & `protobuf-4.23.0rc3/upb/hash/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/hash/int_table.h` & `protobuf-4.23.0rc3/upb/hash/int_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/hash/str_table.h` & `protobuf-4.23.0rc3/upb/hash/str_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json/decode.c` & `protobuf-4.23.0rc3/upb/json/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json/decode.h` & `protobuf-4.23.0rc3/upb/json/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json/encode.c` & `protobuf-4.23.0rc3/upb/json/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json/encode.h` & `protobuf-4.23.0rc3/upb/json/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json_decode.h` & `protobuf-4.23.0rc3/upb/json_decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/json_encode.h` & `protobuf-4.23.0rc3/upb/json_encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/atoi.c` & `protobuf-4.23.0rc3/upb/lex/atoi.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/atoi.h` & `protobuf-4.23.0rc3/upb/lex/atoi.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/round_trip.c` & `protobuf-4.23.0rc3/upb/lex/round_trip.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/round_trip.h` & `protobuf-4.23.0rc3/upb/lex/round_trip.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/strtod.c` & `protobuf-4.23.0rc3/upb/lex/strtod.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/strtod.h` & `protobuf-4.23.0rc3/upb/lex/strtod.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/unicode.c` & `protobuf-4.23.0rc3/upb/lex/unicode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/lex/unicode.h` & `protobuf-4.23.0rc3/upb/lex/unicode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/map.h` & `protobuf-4.23.0rc3/upb/map.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mem/alloc.c` & `protobuf-4.23.0rc3/upb/mem/alloc.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mem/alloc.h` & `protobuf-4.23.0rc3/upb/mem/alloc.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mem/arena.c` & `protobuf-4.23.0rc3/upb/mem/arena.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mem/arena.h` & `protobuf-4.23.0rc3/upb/mem/arena.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mem/arena_internal.h` & `protobuf-4.23.0rc3/upb/mem/arena_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/accessors.c` & `protobuf-4.23.0rc3/upb/message/accessors.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/accessors.h` & `protobuf-4.23.0rc3/upb/message/accessors.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/accessors_internal.h` & `protobuf-4.23.0rc3/upb/message/accessors_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/copy.c` & `protobuf-4.23.0rc3/upb/message/copy.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/copy.h` & `protobuf-4.23.0rc3/upb/message/copy.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/extension_internal.h` & `protobuf-4.23.0rc3/upb/message/extension_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/internal.h` & `protobuf-4.23.0rc3/upb/message/internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/message.c` & `protobuf-4.23.0rc3/upb/message/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/message.h` & `protobuf-4.23.0rc3/upb/message/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/promote.c` & `protobuf-4.23.0rc3/upb/message/promote.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/message/promote.h` & `protobuf-4.23.0rc3/upb/message/promote.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/common.c` & `protobuf-4.23.0rc3/upb/mini_table/common.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/common.h` & `protobuf-4.23.0rc3/upb/mini_table/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/common_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/common_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/decode.c` & `protobuf-4.23.0rc3/upb/mini_table/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/decode.h` & `protobuf-4.23.0rc3/upb/mini_table/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/encode.c` & `protobuf-4.23.0rc3/upb/mini_table/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/encode_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/encode_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/enum_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/enum_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/extension_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/extension_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/extension_registry.c` & `protobuf-4.23.0rc3/upb/mini_table/extension_registry.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/extension_registry.h` & `protobuf-4.23.0rc3/upb/mini_table/extension_registry.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/field_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/field_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/file_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/file_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/message_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/message_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/sub_internal.h` & `protobuf-4.23.0rc3/upb/mini_table/sub_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table/types.h` & `protobuf-4.23.0rc3/upb/mini_table/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/mini_table.h` & `protobuf-4.23.0rc3/upb/mini_table.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/msg.h` & `protobuf-4.23.0rc3/upb/msg.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/msg_internal.h` & `protobuf-4.23.0rc3/upb/msg_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/port/atomic.h` & `protobuf-4.23.0rc3/upb/port/atomic.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/port/def.inc` & `protobuf-4.23.0rc3/upb/port/def.inc`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/port/undef.inc` & `protobuf-4.23.0rc3/upb/port/undef.inc`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/port/vsnprintf_compat.h` & `protobuf-4.23.0rc3/upb/port/vsnprintf_compat.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/common.h` & `protobuf-4.23.0rc3/upb/reflection/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def.h` & `protobuf-4.23.0rc3/upb/reflection/def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_builder.c` & `protobuf-4.23.0rc3/upb/reflection/def_builder.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_builder_internal.h` & `protobuf-4.23.0rc3/upb/reflection/def_builder_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_pool.c` & `protobuf-4.23.0rc3/upb/reflection/def_pool.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_pool.h` & `protobuf-4.23.0rc3/upb/reflection/def_pool.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_pool_internal.h` & `protobuf-4.23.0rc3/upb/reflection/def_pool_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_type.c` & `protobuf-4.23.0rc3/upb/reflection/def_type.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/def_type.h` & `protobuf-4.23.0rc3/upb/reflection/def_type.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/desc_state.c` & `protobuf-4.23.0rc3/upb/reflection/desc_state.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/desc_state_internal.h` & `protobuf-4.23.0rc3/upb/reflection/desc_state_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_def.c` & `protobuf-4.23.0rc3/upb/reflection/enum_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_def.h` & `protobuf-4.23.0rc3/upb/reflection/enum_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/enum_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.c` & `protobuf-4.23.0rc3/upb/reflection/enum_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range.h` & `protobuf-4.23.0rc3/upb/reflection/enum_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_reserved_range_internal.h` & `protobuf-4.23.0rc3/upb/reflection/enum_reserved_range_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_value_def.c` & `protobuf-4.23.0rc3/upb/reflection/enum_value_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_value_def.h` & `protobuf-4.23.0rc3/upb/reflection/enum_value_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/enum_value_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/enum_value_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/extension_range.c` & `protobuf-4.23.0rc3/upb/reflection/extension_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/extension_range.h` & `protobuf-4.23.0rc3/upb/reflection/extension_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/extension_range_internal.h` & `protobuf-4.23.0rc3/upb/reflection/extension_range_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/field_def.c` & `protobuf-4.23.0rc3/upb/reflection/field_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/field_def.h` & `protobuf-4.23.0rc3/upb/reflection/field_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/field_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/field_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/file_def.c` & `protobuf-4.23.0rc3/upb/reflection/file_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/file_def.h` & `protobuf-4.23.0rc3/upb/reflection/file_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/file_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/file_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message.c` & `protobuf-4.23.0rc3/upb/reflection/message.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message.h` & `protobuf-4.23.0rc3/upb/reflection/message.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_def.c` & `protobuf-4.23.0rc3/upb/reflection/message_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_def.h` & `protobuf-4.23.0rc3/upb/reflection/message_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/message_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_reserved_range.c` & `protobuf-4.23.0rc3/upb/reflection/message_reserved_range.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_reserved_range.h` & `protobuf-4.23.0rc3/upb/reflection/message_reserved_range.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/message_reserved_range_internal.h` & `protobuf-4.23.0rc3/upb/reflection/message_reserved_range_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/method_def.c` & `protobuf-4.23.0rc3/upb/reflection/method_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/method_def.h` & `protobuf-4.23.0rc3/upb/reflection/method_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/method_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/method_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/oneof_def.c` & `protobuf-4.23.0rc3/upb/reflection/oneof_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/oneof_def.h` & `protobuf-4.23.0rc3/upb/reflection/oneof_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/oneof_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/oneof_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/service_def.c` & `protobuf-4.23.0rc3/upb/reflection/service_def.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/service_def.h` & `protobuf-4.23.0rc3/upb/reflection/service_def.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/service_def_internal.h` & `protobuf-4.23.0rc3/upb/reflection/service_def_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection/stage0/google/protobuf/descriptor.upb.h` & `protobuf-4.23.0rc3/upb/reflection/stage0/google/protobuf/descriptor.upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/reflection.h` & `protobuf-4.23.0rc3/upb/reflection.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/status.h` & `protobuf-4.23.0rc3/upb/status.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/string_view.h` & `protobuf-4.23.0rc3/upb/string_view.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/text/encode.c` & `protobuf-4.23.0rc3/upb/text/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/text/encode.h` & `protobuf-4.23.0rc3/upb/text/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/text_encode.h` & `protobuf-4.23.0rc3/upb/text_encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/upb.h` & `protobuf-4.23.0rc3/upb/upb.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/compare.c` & `protobuf-4.23.0rc3/upb/util/compare.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/compare.h` & `protobuf-4.23.0rc3/upb/util/compare.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/def_to_proto.c` & `protobuf-4.23.0rc3/upb/util/def_to_proto.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/def_to_proto.h` & `protobuf-4.23.0rc3/upb/util/def_to_proto.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/required_fields.c` & `protobuf-4.23.0rc3/upb/util/required_fields.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/util/required_fields.h` & `protobuf-4.23.0rc3/upb/util/required_fields.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/common.h` & `protobuf-4.23.0rc3/upb/wire/common.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/common_internal.h` & `protobuf-4.23.0rc3/upb/wire/common_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/decode.c` & `protobuf-4.23.0rc3/upb/wire/decode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/decode.h` & `protobuf-4.23.0rc3/upb/wire/decode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/decode_fast.c` & `protobuf-4.23.0rc3/upb/wire/decode_fast.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/decode_fast.h` & `protobuf-4.23.0rc3/upb/wire/decode_fast.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/decode_internal.h` & `protobuf-4.23.0rc3/upb/wire/decode_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/encode.c` & `protobuf-4.23.0rc3/upb/wire/encode.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/encode.h` & `protobuf-4.23.0rc3/upb/wire/encode.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.c` & `protobuf-4.23.0rc3/upb/wire/eps_copy_input_stream.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/eps_copy_input_stream.h` & `protobuf-4.23.0rc3/upb/wire/eps_copy_input_stream.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/reader.c` & `protobuf-4.23.0rc3/upb/wire/reader.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/reader.h` & `protobuf-4.23.0rc3/upb/wire/reader.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/swap_internal.h` & `protobuf-4.23.0rc3/upb/wire/swap_internal.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/upb/wire/types.h` & `protobuf-4.23.0rc3/upb/wire/types.h`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/utf8_range/naive.c` & `protobuf-4.23.0rc3/utf8_range/naive.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/utf8_range/range2-neon.c` & `protobuf-4.23.0rc3/utf8_range/range2-neon.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/utf8_range/range2-sse.c` & `protobuf-4.23.0rc3/utf8_range/range2-sse.c`

 * *Files identical despite different names*

### Comparing `protobuf-4.23.0rc2/utf8_range/utf8_range.h` & `protobuf-4.23.0rc3/utf8_range/utf8_range.h`

 * *Files identical despite different names*

