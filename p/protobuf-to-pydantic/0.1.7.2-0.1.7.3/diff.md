# Comparing `tmp/protobuf_to_pydantic-0.1.7.2.tar.gz` & `tmp/protobuf_to_pydantic-0.1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf_to_pydantic-0.1.7.2.tar", max compression
+gzip compressed data, was "protobuf_to_pydantic-0.1.7.3.tar", max compression
```

## Comparing `protobuf_to_pydantic-0.1.7.2.tar` & `protobuf_to_pydantic-0.1.7.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.1.7.2/LICENSE
--rw-r--r--   0        0        0    33623 2023-03-23 17:23:44.348493 protobuf_to_pydantic-0.1.7.2/README.md
--rw-r--r--   0        0        0      157 2023-04-06 10:17:44.904269 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/__init__.py
--rw-r--r--   0        0        0       25 2023-04-17 15:19:23.715975 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/__version__.py
--rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/contrib/__init__.py
--rw-r--r--   0        0        0    14814 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/contrib/proto_parser.py
--rw-r--r--   0        0        0     7873 2022-08-19 06:41:43.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/customer_con_type.py
--rw-r--r--   0        0        0    11699 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/customer_validator.py
--rw-r--r--   0        0        0    23973 2023-04-17 15:18:55.763482 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/gen_code.py
--rw-r--r--   0        0        0    28283 2023-04-09 15:30:54.888047 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/gen_model.py
--rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/__init__.py
--rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
--rw-r--r--   0        0        0    14497 2023-03-30 12:19:52.880142 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/base.py
--rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
--rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
--rw-r--r--   0        0        0     2074 2022-07-30 20:12:53.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/types.py
--rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_proto_file.py
--rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pyi_file.py
--rw-r--r--   0        0        0     1517 2023-03-30 17:36:31.267633 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/grpc_types.py
--rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/__init__.py
--rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/__main__.py
--rw-r--r--   0        0        0     3508 2023-04-01 17:20:07.477049 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/code_gen.py
--rw-r--r--   0        0        0     2482 2023-03-30 07:29:18.237163 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/config.py
--rw-r--r--   0        0        0    19774 2023-04-17 15:18:55.767482 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
--rwxr-xr-x   0        0        0      347 2023-03-30 03:00:46.463995 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/main.py
--rw-r--r--   0        0        0      332 2023-02-22 17:08:00.346785 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/my_types.py
--rw-r--r--   0        0        0   383358 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   185862 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-16 17:55:03.519814 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0   121461 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-16 17:55:03.515814 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-16 17:52:05.182463 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0    34121 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   185862 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-16 17:55:03.499814 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0    13083 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-04-16 17:55:03.499814 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-04-16 17:52:23.654605 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/validate_pb2.py
--rw-r--r--   0        0        0     1593 2023-02-22 16:09:35.749710 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/types.py
--rw-r--r--   0        0        0     5755 2023-04-16 17:46:30.623748 protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/util.py
--rw-r--r--   0        0        0     3109 2023-04-17 15:19:23.715975 protobuf_to_pydantic-0.1.7.2/pyproject.toml
--rw-r--r--   0        0        0    35927 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.2/setup.py
--rw-r--r--   0        0        0    34841 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.1.7.3/LICENSE
+-rw-r--r--   0        0        0    33623 2023-03-23 17:23:44.348493 protobuf_to_pydantic-0.1.7.3/README.md
+-rw-r--r--   0        0        0      157 2023-04-06 10:17:44.904269 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-08 14:46:25.624494 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/__version__.py
+-rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/contrib/__init__.py
+-rw-r--r--   0        0        0    14814 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/contrib/proto_parser.py
+-rw-r--r--   0        0        0     7873 2022-08-19 06:41:43.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/customer_con_type.py
+-rw-r--r--   0        0        0    11699 2023-03-19 16:10:34.117082 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/customer_validator.py
+-rw-r--r--   0        0        0    24075 2023-05-08 14:45:26.935905 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/gen_code.py
+-rw-r--r--   0        0        0    28283 2023-05-06 19:22:29.572484 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/gen_model.py
+-rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/__init__.py
+-rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
+-rw-r--r--   0        0        0    14497 2023-05-06 19:22:29.572484 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/base.py
+-rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
+-rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
+-rw-r--r--   0        0        0     2074 2022-07-30 20:12:53.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/types.py
+-rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_proto_file.py
+-rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pyi_file.py
+-rw-r--r--   0        0        0     1517 2023-05-06 19:22:29.572484 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/grpc_types.py
+-rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/__main__.py
+-rw-r--r--   0        0        0     3508 2023-04-01 17:20:07.477049 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/code_gen.py
+-rw-r--r--   0        0        0     2482 2023-05-06 19:22:29.572484 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/config.py
+-rw-r--r--   0        0        0    19759 2023-05-08 14:44:17.270399 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
+-rwxr-xr-x   0        0        0      347 2023-03-30 03:00:46.463995 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/main.py
+-rw-r--r--   0        0        0      332 2023-05-06 19:22:29.572484 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/my_types.py
+-rw-r--r--   0        0        0   383358 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   185862 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-06 19:26:23.563279 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0   121461 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-06 19:26:23.575279 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-06 19:24:53.321322 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0    34121 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   185862 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-06 19:26:23.575279 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13083 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-05-06 19:26:23.579279 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-06 19:25:34.496115 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/validate_pb2.py
+-rw-r--r--   0        0        0     1593 2023-02-22 16:09:35.749710 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/types.py
+-rw-r--r--   0        0        0     5755 2023-04-21 11:21:31.226554 protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/util.py
+-rw-r--r--   0        0        0     3109 2023-05-08 14:46:25.624494 protobuf_to_pydantic-0.1.7.3/pyproject.toml
+-rw-r--r--   0        0        0    35927 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.3/setup.py
+-rw-r--r--   0        0        0    34841 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.1.7.3/PKG-INFO
```

### Comparing `protobuf_to_pydantic-0.1.7.2/LICENSE` & `protobuf_to_pydantic-0.1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/README.md` & `protobuf_to_pydantic-0.1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/contrib/proto_parser.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/contrib/proto_parser.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/customer_con_type.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/customer_con_type.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/customer_validator.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/customer_validator.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/gen_code.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/gen_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,33 +97,35 @@
         if module_name in (gen_model.__name__, __name__):
             return
         if class_name:
             self._import_set.add(f"from {module_name} import {class_name}{extra_str}")
         else:
             self._import_set.add(f"import {module_name}")
 
-    def _get_value_code(self, type_: Any, auto_import_type_code: bool = True) -> str:
+    def _get_value_code(self, type_: Any, auto_import_type_code: bool = True, sort: bool = True) -> str:
         """
         Get the output string corresponding to the type
         :param type_: needs to be parsed type
         :param auto_import_type_code: If True, will generate by the way import code
+        :param sort: If True, will sort item (Ensure that the order of code generated multiple times is consistent)
         :return:
         """
         type_ = replace_protobuf_type_to_python_type(type_)
         if isinstance(type_, dict):
             sort_list: list = [(k, v) for k, v in type_.items()]
-            # Ensure that the order of code generated multiple times is consistent
-            sort_list.sort()
+            if sort:
+                sort_list.sort()
             type_name: str = ", ".join(
                 sorted([f"{self._get_value_code(k)}: {self._get_value_code(v)}" for k, v in sort_list])
             )
             return "{" + type_name + "}"
         elif isinstance(type_, (list, tuple, set)):
             sort_list = [self._get_value_code(i) for i in type_]
-            sort_list.sort()
+            if sort:
+                sort_list.sort()
             type_name = ", ".join(sort_list)
             if isinstance(type_, list):
                 return "[" + type_name + "]"
             elif isinstance(type_, set):
                 return "{" + type_name + "}"
             else:
                 return "(" + type_name + ")"
```

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/gen_model.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/gen_model.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/base.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/base.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pb_option/types.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pb_option/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_proto_file.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_proto_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/get_desc/from_pyi_file.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/get_desc/from_pyi_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/grpc_types.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/grpc_types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/code_gen.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/code_gen.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/config.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/config.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,16 +262,16 @@
             type_str = f"typing.Dict[{key_type_str}, {value_type_str}]"
 
         # custom field support
         field_class: Optional[FieldInfo] = field_info_dict.pop("field", None)
         if field_class:
             field_name: str = self._get_value_code(field_class)
         else:
-            field_name = "FieldInfo"
-            self._add_import_code("pydantic.fields", "FieldInfo")
+            field_name = "Field"
+            self._add_import_code("pydantic", "Field")
 
         # arranging  field info parameters
         for key in FieldInfo.__slots__:
             value: Any = field_info_dict.get(key, None)
             if value is getattr(FieldInfo(), key):
                 field_info_dict.pop(key, None)
```

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/protos/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/protos/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/types.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/protobuf_to_pydantic/util.py` & `protobuf_to_pydantic-0.1.7.3/protobuf_to_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.1.7.2/pyproject.toml` & `protobuf_to_pydantic-0.1.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protobuf_to_pydantic"
-version = "v0.1.7.2"
+version = "v0.1.7.3"
 description = "Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/protobuf_to_pydantic"
 homepage = "https://github.com/so1n/protobuf_to_pydantic"
 packages = [
```

### Comparing `protobuf_to_pydantic-0.1.7.2/setup.py` & `protobuf_to_pydantic-0.1.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 entry_points = \
 {'console_scripts': ['protoc-gen-protobuf-to-pydantic = '
                      'protobuf_to_pydantic.plugin.main:main']}
 
 setup_kwargs = {
     'name': 'protobuf-to-pydantic',
-    'version': '0.1.7.2',
+    'version': '0.1.7.3',
     'description': 'Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum',
     'long_description': '# protobuf_to_pydantic\nGenerate the `pydantic.Base Model` class (and the corresponding source code) with parameter verification function through the Protobuf file\n\n> NOTE:\n>  - Only supports proto3\n\n[中文文档](https://github.com/so1n/protobuf_to_pydantic/blob/master/README_ZH.md)\n# 1.Installation\n```bash\npip install protobuf_to_pydantic\n```\n\n# 2.Quick Start\n`protobuf_to_pydantic` currently has two methods to generate `pydantic.BaseModel` objects through Protobuf files,\nThe first method is to generate the corresponding `Python` code file through the Protobuf file in the form of a plugin.\nThe second method is to generate the corresponding `pydantic.BaseModel` object based on the `Message` object at runtime.\n\n## 2.1.Directly generate `pydantic.BaseModel` code files through plugins\n> Note: The `protobuf-to-pydantic` plugin depends on `mypy-protobuf`, please install `mypy-protobuf` through the command `python -m pip install protobuf-to-pydanitc[mypy-protobuf]`.\n### 2.1.1.Use of plugin\nThe plugin method is the most recommended way to use `protobuf-to-pydantic`,\nit supports the most complete functions, and it is also very simple to use, assuming that the code corresponding to the Protobuf file is usually generated by the following command:\n```bash\npython -m grpc_tools.protoc -I. example.proto\n```\nThen after installing `protobuf-to-pydantic`, can use the `--protobuf-to-pydantic out` option to use `protobuf-to-pydantic`, the command is as follows:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto\n```\n\nAmong them, `--protobuf-to-pydantic out=.` indicates the use of the `prorobuf-to-pydanitc` plugin, and declares that the output location of the `protobuf-to-pydantic` plugin is `.` (indicating the use of `grpc tools.proto ` to use the output path),\nIn this way, the `protobuf-to-pydantic` plugin will write its own generated content in the corresponding file (the file name ends with `p2p.py`), such as `protobuf-to-pydantic` is `example.proto `The generated code file is named `example_p2p.py`\n\n### 2.1.2.Plugin configuration\n`protobuf-to-pydantic` supports configuration functions by reading a `Python` file.\nDevelopers first need to create a configuration file in the current path of the running command, the file name is `plugin_config.py`, and write the following code:\n```Python\nimport logging\nfrom typing import List, Type\n\nfrom google.protobuf.any_pb2 import Any  # type: ignore\nfrom pydantic import confloat, conint\nfrom pydantic.fields import FieldInfo\n\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\n# Configure the log output format and log level of the plugin, which is very useful when debugging\nlogging.basicConfig(format="[%(asctime)s %(levelname)s] %(message)s", datefmt="%y-%m-%d %H:%M:%S", level=logging.DEBUG)\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\ndef customer_any() -> Any:\n    return Any  # type: ignore\n\n\n# For the configuration of the local template, see the use of the local template for details\nlocal_dict = {\n    "CustomerField": CustomerField,\n    "confloat": confloat,\n    "conint": conint,\n    "customer_any": customer_any,\n}\n# Specifies the start of key comments\ncomment_prefix = "p2p"\n# Specify the class of the template, you can extend the template by inheriting this class, see the chapter on custom templates for details\ndesc_template: Type[DescTemplate] = DescTemplate\n# Specify the protobuf files of which packages to ignore, and the messages of the ignored packages will not be parsed\nignore_pkg_list: List[str] = ["validate", "p2p_validate"]\n# Specifies the generated file name suffix (without .py)\nfile_name_suffix = "_p2p"\n```\nNext, change `--protobuf-to-pydantic out=.` in the command to `--protobuf-to-pydantic out=config path=plugin config.py:.`, as follows:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n```\nAmong them, `config path=plugin_config.py` on the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` still declares the output of the `protobuf-to-pydantic` plugin The position is `.`.\nIn this way, the `protobuf-to-pydantic` plugin can be loaded into the configuration file specified by the developer when it is running, and then run according to the configuration defined by the configuration file.\n\n> Note: 更多配置内容见`protobuf_to_pydantic/plugin/config.py`文件\n> Note: For more information on configuration, see the \'protobuf_to_pydantic/plugin/config.py\'\n## 2.2.Generate a `pydantic.BaseModel` object at runtime\n`protobuf_to_pydantic` can generate the corresponding `pydantic.BaseModel` object based on the `Message` object at runtime。\n\nFor example, the `UserMessage` in the following Protobuf file named `demo.proto`:\n```protobuf\n// path: ./demo.proto\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\nmessage UserMessage {\n  string uid=1;\n  int32 age=2;\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  string user_name=6;\n}\n```\nThrough `grpc_tools.protoc`, the corresponding `Python` code can be generated according to the Protobuf file (the file name at this time is `demo_pb2.py`),\nand the `msg_to_pydantic_model` method of `protobuf_to_pydantic` can read the generated Proto file at runtime Message object data,\nand generate the corresponding `pydantic.BaseModel` object:\n\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom . import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n\n# output\n# {\n#   \'uid\': FieldInfo(default=\'\', extra={}),\n#   \'age\': FieldInfo(default=0, extra={}),\n#   \'height\': FieldInfo(default=0.0, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', extra={})\n#  }\n```\nThrough the output results, it can be found that the generated `pydantic.BaseModel` object also contains `uid`, `age`, `height`, `sex`, `is adult` and `user name` fields, and their corresponding `default` The information is consistent with the `UserMessage` in the Protobuf file.\n\nIn addition to generating the corresponding `pydantic.BaseModel` object at runtime, `protobuf-to-pydantic` also supports converting the `pydantic.BaseModel` object to the corresponding `Python` code text at runtime (only compatible with `protobuf_to_pydantic `generated `pydantic.BaseModel` object).\nAmong them, the `pydantic_model_to_py_code` method of `protobuf_to_pydantic` is used to generate code text, and the `pydantic_model_to_py_file` method of `protobuf_to_pydantic` is used to generate code files,\nthe sample code of `pydantic_model_to_py_file` method of `protobuf_to_pydantic` is as follows:\n```Python\nfrom protobuf_to_pydantic import msg_to_pydantic_model, pydantic_model_to_py_file\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\npydantic_model_to_py_file(\n    "./demo_gen_code.py",\n    msg_to_pydantic_model(demo_pb2.NestedMessage),\n)\n```\nThe code will first convert `demo_pb2.NestedMessage` into a `pydantic.BaseModel` object, and then the generated object will be converted into the corresponding code content by the `pydantic_model_to_py_file` method and written to `demo_gen_code.py` file.\n\n## 2.3.Parameter verification\nThe `Message` object generated according to the Protobuf file will only carry a small amount of information. This is because the ordinary Protobuf file does not have enough parameter verification related information, which requires us to improve the parameter verification information of the `Message` object through some additional ways.\nCurrently `protobuf_to_pydantic` supports multiple ways to obtain other information of the Message, so that the generated `pydantic.BaseModel` object has the function of parameter verification.\n\n> NOTE:\n>  - 1.The text annotation function is not the focus of subsequent function development, and the P2P mode is recommended。\n>  - 2.Plugin mode only supports PGV and P2P mode\n\n### 2.3.1.Text annotation\nDevelopers can write comments that meet the requirements of `protobuf_to_pydantic` for each field in the Protobuf file to provide parameter verification information for `protobuf_to_pydantic`, such as the following example:\n```protobuf\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\n// user info\nmessage UserMessage {\n  // p2p: {"miss_default": true, "example": "10086"}\n  // p2p: {"title": "UID"}\n  string uid=1; // p2p: {"description": "user union id"}\n  // p2p: {"example": 18, "title": "use age", "ge": 0}\n  int32 age=2;\n  // p2p: {"ge": 0, "le": 2.5}\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  // p2p: {"description": "user name"}\n  // p2p: {"default": "", "min_length": 1, "max_length": "10", "example": "so1n"}\n  string user_name=6;\n}\n```\nIn this example, each annotation that can be used by `protobuf_to_pydantic` starts with `p2p:` (supports customization) and is followed by a complete Json string. If you are familiar with the usage of `pydantic`, you can find This Json string contains the verification information corresponding to `pydantic.Field`. For example, the `uid` field in `UserMessage` contains a total of 4 pieces of information as follows：\n\n| Column       | Meaning                                                                               |\n|--------------|---------------------------------------------------------------------------------------|\n| miss_default | Indicates that the generated field does not have a default value                      |\n| example      | An example value representing the generated field is 10086                            |\n| title        | Indicates that the schema name of the field is UID                                    |\n | description  | The schema documentation for the representation field is described as `user_union_id` |\n\n> Note:\n>   - 1.Currently only single-line comments are supported and comments must be a complete Json data (no line breaks).\n>   - 2.multi line comments are not supported。\n\nWhen these annotations are written, `protobuf_to_pydantic` will bring the corresponding information for each field when converting the Message into the corresponding `Pydantic.BaseModel` object, as follows:\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage, parse_msg_desc_method=demo_pb2)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'uid\': FieldInfo(default=PydanticUndefined, title=\'UID\', description=\'user union id\', extra={\'example\': \'10086\'}),\n#   \'age\': FieldInfo(default=0, title=\'use age\', ge=0, extra={\'example\': 18}),\n#   \'height\': FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', description=\'user name\', min_length=1, max_length=10, extra={\'example\': \'so1n\'})\n# }\n```\nIt can be seen from the output results that the output fields carry the corresponding information. In addition, the difference between this code and the above is that the `msg_to_pydantic_model` function sets a keyword parameter named `parse_msg_desc_method` and its value is `demo_pb2`, which enables `protobuf_to_pydantic` to obtain additional information for each field in the Message object through comments in the `.pyi` file of the `demo_pb2` module.\n\n> Note：This function requires the use of the [mypy-protobuf](https://github.com/nipunn1313/mypy-protobuf) plugin when generating the corresponding `Python` code from the Protobuf file, and the specified output path of the pyi file is the same as the generated `Python` code path to take effect at the same time.\n\nIn addition to obtaining comments through the `.pyi` file, `protobuf_to_pydantic` also supports setting the value of `parse_msg_desc_method` to the root directory path specified when the Message object is generated, so that `protobuf_to_pydantic` can parse the comments of the Protobuf file corresponding to the Message object. getting information。\n\n\nFor example, the project structure of the `protobuf_to_pydantic` sample code is as follows:\n```bash\n./protobuf_to_pydantic/\n├── example/\n│ ├── python_example_proto_code/\n│ └── example_proto/\n├── protobuf_to_pydantic/\n└── /\n```\n\nThe Protobuf file is stored in the `example/example_proto` folder, and then run the following command in the `example` directory to generate the `Python` code file corresponding to Protobuf:\n```bash\ncd example\n\npython -m grpc_tools.protoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n```\nThen the path to be filled in at this time is `./protobuf_to_pydantic/example`, the code is as follows：\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.UserMessage, parse_msg_desc_method="./protobuf_to_pydantic/example"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'uid\': FieldInfo(default=PydanticUndefined, title=\'UID\', description=\'user union id\', extra={\'example\': \'10086\'}),\n#   \'age\': FieldInfo(default=0, title=\'use age\', ge=0, extra={\'example\': 18}),\n#   \'height\': FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   \'sex\': FieldInfo(default=0, extra={}),\n#   \'is_adult\': FieldInfo(default=False, extra={}),\n#   \'user_name\': FieldInfo(default=\'\', description=\'user name\', min_length=1, max_length=10, extra={\'example\': \'so1n\'})\n# }\n```\nFrom the result, it can be seen that the information carried by the field is the same as the result obtained by the module\n> NOTE: This method requires [lark](https://github.com/lark-parser/lark) to be installed in advance and the Protobuf file must exist in the running project.\n\n### 2.3.2.PGV(protoc-gen-validate)\nCurrently, the commonly used object validation method in the Protobuf ecosystem is to directly use the [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) project, while [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) project also supports multiple languages, and most Protobuf developers will write `pgv` rules once so that different languages support the same validation rules.\n\nAnd `protobuf-to-pydantic` also supports parsing the verification rules of `pgv` so that the generated `pydantic.BaseModel` class has corresponding verification logic,\nIt is very simple to use `Pgv` verification rules in `protobuf_to_pydantic`. First, you need to write the corresponding `Pgv` rules in the Protobuf file, and then fill in `parse_msg_desc_method` when converting through `msg_to_pydantic_model` method The value is `PGV`, the code is as follows:\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.validate import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest, parse_msg_desc_method="PGV"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'ignore_test\': FieldInfo(default=0.0, extra={})\n# }\n```\n\n> Note:\n>  - 1.For the usage of `Pgv`, see: [protoc-gen-validate doc](https://github.com/bufbuild/protoc-gen-validate/blob/main/README.md#constraint-rules)\n>  - 2.Need to install `Pgv` through `pip install protoc_gen_validate` Or download [validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/common/validate.proto) to the protobuf directory in the project to write pgv rules in the Protobuf file.\n\n\n### 2.2.3.P2p\nThe verification rules of `Pgv` are written in the Option attribute of each field of `Message`, and there are better code specifications, so the readability of Protobuf files carrying `Pgv` verification rules is higher than that of Protobuf carrying comments At the same time, when writing `Pgv` rules, you can also experience the convenience brought by IDE auto-completion, but it only supports verification-related logic, and the feature richness is not as good as the file comment mode.\n\nThe `P2P` mode is an extension of the `PGV` mode, which incorporates some functions of text annotations. This mode satisfies the customization of the attributes of each `Field` in most `pydantic.BaseModel`, such as the following Protobuf file:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\n\nimport "example_proto/common/p2p_validate.proto";\n\n\nmessage FloatTest {\n  float const_test = 1 [(p2p_validate.rules).float.const = 1];\n  float range_e_test = 2 [(p2p_validate.rules).float = {ge: 1, le: 10}];\n  float range_test = 3[(p2p_validate.rules).float = {gt: 1, lt: 10}];\n  float in_test = 4[(p2p_validate.rules).float = {in: [1,2,3]}];\n  float not_in_test = 5[(p2p_validate.rules).float = {not_in: [1,2,3]}];\n  float default_test = 6[(p2p_validate.rules).float.default = 1.0];\n  float not_enable_test = 7[(p2p_validate.rules).float.enable = false];\n  float default_factory_test = 8[(p2p_validate.rules).float.default_factory = "p2p@builtin|float"];\n  float miss_default_test = 9[(p2p_validate.rules).float.miss_default = true];\n  float alias_test = 10 [(p2p_validate.rules).float.alias = "alias"];\n  float desc_test = 11 [(p2p_validate.rules).float.description = "test desc"];\n  float multiple_of_test = 12 [(p2p_validate.rules).float.multiple_of = 3.0];\n  float example_test = 13 [(p2p_validate.rules).float.example = 1.0];\n  float example_factory = 14 [(p2p_validate.rules).float.example_factory = "p2p@builtin|float"];\n  float field_test = 15[(p2p_validate.rules).float.field = "p2p@local|CustomerField"];\n  float type_test = 16[(p2p_validate.rules).float.type = "p2p@local|confloat"];\n  float title_test = 17 [(p2p_validate.rules).float.title = "title_test"];\n}\n```\n`protobuf_to_pydantic` can read the generated Message object at runtime and generate a `pydantic.BaseModel` object with the corresponding information:\n\n```python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel, confloat\nfrom pydantic.fields import FieldInfo\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.p2p_validate import demo_pb2\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\nDemoModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest,\n    local_dict={"CustomerField": CustomerField, "confloat": confloat},\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in DemoModel.__fields__.items()\n    }\n)\n# output:\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'default_test\': FieldInfo(default=1.0, extra={}),\n#   \'default_factory_test\': FieldInfo(default=PydanticUndefined, default_factory=<class \'float\'>, extra={}),\n#   \'miss_default_test\': FieldInfo(extra={}),\n#   \'alias_test\': FieldInfo(default=0.0, alias=\'alias\', alias_priority=2, extra={}),\n#   \'desc_test\': FieldInfo(default=0.0, description=\'test desc\', extra={}),\n#   \'multiple_of_test\': FieldInfo(default=0.0, multiple_of=3, extra={}),\n#   \'example_test\': FieldInfo(default=0.0, extra={\'example\': 1.0}),\n#   \'example_factory\': FieldInfo(default=0.0, extra={\'example\': <class \'float\'>}),\n#   \'field_test\': CustomerField(default=0.0, extra={}),\n#   \'type_test\': FieldInfo(default=0.0, extra={}),\n#   \'title_test\': FieldInfo(default=0.0, title=\'title_test\', extra={})\n#   }\n```\nIt is worth noting that this code does not explicitly specify that the value of `parse_msg_desc_method` is `p2p`, because `p2p` is already the default rule of `protobuf_to_pydantic`.\n\n> Note: See the template chapter for the usage of `local_dict`\n\n > Note:\n>  - 1.See the template chapter for the usage of `local_dict`\n>  - 2.If the reference to the Proto file fails, you need to download [p2p_validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/protos/protobuf_to_pydantic/protos/p2p_validate.proto) in the project and use it in the Protobuf file。\n\n\n\n\n### 2.3.3.Other parameter support\nIn addition to the parameters of `FieldInfo`, the file comment mode and `p2p` mode of `protobuf_to_pydantic` also support the following parameters:\n- miss_default：By default, the default value of each field in the corresponding `pydantic.BaseModel` object is the same as the default value of each field in the Message, but when `miss default` is `true`, the setting of the default value will be canceled .\n- enable: By default, `pydantic.BaseModel` will convert every field in the Message. If some fields do not want to be converted, you can set `enable` to `false`\n- const: Specifies the value of the field\'s constant. Note: The const of `pydantic.BaseModel` only supports bool variables. When `const` is `True`, the accepted value can only be the value set by `default`, and the default value carried by the Message generated by protobuf corresponds to The null value of type does not match `pydantic.BaseModel`, so `protobuf_to_pydantic` makes some changes to the input of this value, but after `const` sets the value, the `cost` property in the generated field is `True` `, and `default` becomes the corresponding value of the setting.\n- type: To expand the current type, for example, if you want to increase the verification of the bank card number through the `pydantic.types.Payment Card Number` type, you can specify the field type as `Payment Card Number` by the following method:\n  ```protobuf\n  // common example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  // p2p example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n> Note:\n>   If you don\'t know `pydantic`, you can use the following two URLs to learn what parameters Field supports:\n>\n>   - https://pydantic-docs.helpmanual.io/usage/types/#constrained-types\n>\n>   - https://pydantic-docs.helpmanual.io/usage/schema/#field-customization\n\n### 2.3.4.Template\nIn some cases, the value we fill in is a method or function of a certain library in `Python` (such as the value of `type` parameter and `default_factory` parameter), which cannot be realized through Json syntax。\nAt this time, template parameters can be used to solve the corresponding problems. Currently `protobuf_to_pydantic` supports a variety of template parameters。\n\n> Note:The `p2p` string at the beginning of the template can be defined by the comment prefix variable\n\n\n#### 2.3.4.1.`p2p@import`\nThis template is used to indicate that the value is a variable under other modules. The specific usage method is as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n}\n\n// p2p example\nmessage UserPayMessage {\n  string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n}\n\n// p2p other example\n// Since the imported type happens to belong to the `pydantic.types` module, string.pydantic type can be used directly in `p2p` mode\nmessage UserPayMessage {\n  string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n}\n```\n\nThe syntax in the format of `p2p{template method}|{module to be imported: A}|{variable in the module: B}` is used here, which means that `B` object needs to be imported and applied through `from A import B` ,\nThrough the definition of the template, `protobuf_to_pydantic` will convert the corresponding Message into the following `pydantic.BaseModel`:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n# p2p@import|pydantic.types|PaymentCardNumber\nfrom pydantic.types import PaymentCardNumber\n\nclass UserPayMessage(BaseModel):\n    bank_number: PaymentCardNumber = FieldInfo(default="", extra={})\n```\n\n#### 2.3.4.2.`p2p@import_instance`\nThe `p2p@import` template just imports and uses the variables of a certain library, while `p2p@import instance` imports the class of a certain library first,\nand finally instantiates it with the specified parameters. The method of use is as follows:\n```protobuf\nmessage AnyTest {\n  google.protobuf.Any default_test = 23 [\n    (p2p_validate.rules).any.default = \'p2p@import_instance|google.protobuf.any_pb2|Any|{"type_url": "type.googleapis.com/google.protobuf.Duration"}\'\n\n  ];\n}\n```\nHere is the `p2p{template method}|{module to be imported}|{corresponding class}|{corresponding parameter}` syntax, through the definition of the template, `protobuf_to_pydantic` will convert the corresponding Message is the following `pydantic.BaseModel` object:\n```python\nfrom google.protobuf.any_pb2 import Any as AnyMessage\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass AnyTest(BaseModel):\n    default_test: AnyMessage = FieldInfo(\n        default=AnyMessage(type_url="type.googleapis.com/google.protobuf.Duration")\n    )\n```\n\n#### 2.3.4.3.`p2p@local`\nThis template is used to introduce user-defined variables. The syntax in the format `{template method}|{local variable to be used}` is used here, as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1; // p2p: {"default_factory": "p2p@local|exp_time"}\n}\n// p2p example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.default_factory= "p2p@local|exp_time"];\n}\n```\nThen register the corresponding value through the parameter `local_dict` when calling the `msg_to_pydantic_model` method. The fake code is as follows:\n```Python\nimport time\n\n\ndef exp_time() -> float:\n  return time.time()\n\nmsg_to_pydantic_model(\n    demo_pb2.NestedMessage,\n    local_dict={"exp_time": exp_time},  # <----\n)\n```\nIn this way, `protobuf_to_pydantic` can generate a `pydantic.BaseModel` object that meets the requirements:\n```python\nfrom datetime import datetime\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nfrom . import exp_time\n\nclass UserPayMessage(BaseModel):\n    exp: datetime = FieldInfo(default_factory=exp_time, extra={})\n```\n\n> Note: See the sample code for specific calling and generation methods.\n\n#### 2.3.4.4.`p2p@builtin`\nWhen the variable to be used comes from a built-in function, this template can be used directly (it can be considered as a simplified version of the `p2p@local` template), and the syntax is as follows:\n```protobuf\n// comment example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1; // p2p: {"type": "p2p@builtin|float"}\n}\n\n// p2p example\nmessage UserPayMessage {\n  google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.type= "p2p@builtin|float"];\n}\n```\nIn this way, `protobuf_to_pydantic` can generate a `pydantic.BaseModel` object that meets the requirements:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass UserPayMessage(BaseModel):\n    exp: float = FieldInfo()\n```\n#### 2.3.4.5.Custom template\nCurrently, `protobuf_to_pydantic` only supports several templates. If you have more template requirements, you can extend the template by inheriting the `DescTemplate` class.\nFor example, there is a strange requirement that the default value of the field is the timestamp when the Message object is generated as a `pydantic.BaseModel` object, but the timestamp has two versions, one version has a timestamp of length 10 and the other has a length of 13, so write the following Protobuf file:\n```protobuf\nmessage TimestampTest{\n  int32 timestamp_10 = 1[(p2p_validate.rules).int32.default = "p2p@timestamp|10"];\n  int32 timestamp_13 = 2[(p2p_validate.rules).int32.default = "p2p@timestamp|13"];\n}\n```\nThis file uses the custom `p2p@timestamp|{x}` syntax, where `x` only has two values of 10 and 13, and then you can write code according to this template behavior, the code is as follows:\n```python\nimport time\nfrom typing import Any, List\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\n\nclass CustomDescTemplate(DescTemplate):\n    def template_timestamp(self, template_var_list: List[str]) -> Any:\n        timestamp: float = time.time()\n        length: str = template_var_list[0]\n        if length == "10":\n            return int(timestamp)\n        elif length == "13":\n            return int(timestamp * 100)\n        else:\n            raise KeyError(f"timestamp template not support value:{length}")\n\n\nfrom .demo_pb2 import TimestampTest # fake code\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\nmsg_to_pydantic_model(\n    TimestampTest,\n    desc_template=CustomDescTemplate\n)\n```\nThis code first creates a `CustomDescTemplate` class inherited from `DescTemplate`, and this class adds a `template_timestamp` method to match the syntax of `p2p@timestamp`,\nThen specify the template class as `CustomDescTemplate` through the `desc_template` key parameter in `msg_to_pydantic_model`, so that `msg_to_pydantic_model` will generate the following code (assuming the code generated when the timestamp is 1600000000 ):\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nclass TimestampTest(BaseModel):\n    timestamp_10: int = FieldInfo(default=1600000000)\n    timestamp_13: int = FieldInfo(default=1600000000000)\n```\n\n## 3.Code formatting\nCode generated directly via `protobuf_to_pydantic` is not perfect, but `protobuf+type_pydantic` can rely on different formatting tools to generate code that conforms to the `Python` specification.\nCurrently supported formatting tools are `autoflake`, `black` and `isort`, but the prerequisite for using these tools is that the corresponding formatting tools are installed in the current running environment.\n\nIn addition, developers can decide how the formatter will execute through the `pyproject.toml` configuration file, an example of `pyproject.toml` as follows:\n```toml\n# Controls which formatters protobuf-to-pydantic can use, false means that the formatter is not used (default is true)\n[tool.protobuf-to-pydantic.format]\nblack = true\nisort = true\nautoflake = true\n\n# See the black configuration documentation:https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format\n[tool.black]\nline-length = 120\ntarget-version = [\'py37\']\n\n# See the isort configuration documentation:https://pycqa.github.io/isort/docs/configuration/config_files.html#pyprojecttoml-preferred-format\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\ninclude_trailing_comma = true\nforce_grid_wrap = 0\nuse_parentheses = true\nensure_newline_before_comments = true\nline_length = 120\n\n# See the autoflake configuration documentation:https://github.com/PyCQA/autoflake#configuration\n[tool.autoflake]\nin-place = true\nremove-all-unused-imports = true\nremove-unused-variables = true\n```\n\n## 4.example\n`protobuf_to_pydantic` provides some simple sample code, the following is the path of the sample code and protobuf file, just for reference:\n\n| Implication                           | Example Protobuf                                                                            | Example code                                                                         |\n|------------------------------|---------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------|\n| Generate Model code with validation rules based on p2p schema | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/p2p_validate | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/p2p_validate_example |\n| Generate the basic Model code               | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/demo         | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/simple_example      |\n| Generate Model code with validation rules from .pyi files     | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/demo         | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/text_comment_example |\n| Generate Model code with validation rules from protobuf files | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/example_proto/validate     | https://github.com/so1n/protobuf_to_pydantic/tree/master/example/validate_example    |\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/protobuf_to_pydantic',
```

### Comparing `protobuf_to_pydantic-0.1.7.2/PKG-INFO` & `protobuf_to_pydantic-0.1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf-to-pydantic
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: Convert Protobuf-generated Python objects to Pydantic.BaseModel objects with parameter checksum
 Home-page: https://github.com/so1n/protobuf_to_pydantic
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

