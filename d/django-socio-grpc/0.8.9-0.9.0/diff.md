# Comparing `tmp/django-socio-grpc-0.8.9.tar.gz` & `tmp/django-socio-grpc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-socio-grpc-0.8.9.tar", max compression
+gzip compressed data, was "django-socio-grpc-0.9.0.tar", max compression
```

## Comparing `django-socio-grpc-0.8.9.tar` & `django-socio-grpc-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/LICENSE
--rw-r--r--   0        0        0       20 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/__init__.py
--rw-r--r--   0        0        0      352 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/apps.py
--rw-r--r--   0        0        0     5268 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/exceptions.py
--rw-r--r--   0        0        0     9172 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/generics.py
--rw-r--r--   0        0        0     1928 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/log.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/management/__init__.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/management/commands/__init__.py
--rw-r--r--   0        0        0     7128 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/management/commands/generateproto.py
--rw-r--r--   0        0        0     5110 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/management/commands/grpcrunaioserver.py
--rw-r--r--   0        0        0     5314 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/management/commands/grpcrunserver.py
--rw-r--r--   0        0        0    12272 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/mixins.py
--rw-r--r--   0        0        0     4376 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/proto_serializers.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/protobuf/__init__.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/protobuf/default_generated_data.py
--rw-r--r--   0        0        0    11086 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/protobuf/generators.py
--rw-r--r--   0        0        0      420 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/protobuf/json_format.py
--rw-r--r--   0        0        0       97 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/request_transformer/__init_.py
--rw-r--r--   0        0        0     2535 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/request_transformer/grpc_socio_proxy_context.py
--rw-r--r--   0        0        0     3893 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/servicer_proxy.py
--rw-r--r--   0        0        0     3136 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/services.py
--rw-r--r--   0        0        0     4744 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/settings.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/__init__.py
--rw-r--r--   0        0        0     7886 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/assets/generated_protobuf_files.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/__init__.py
--rw-r--r--   0        0        0      146 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/apps.py
--rw-r--r--   0        0        0     4005 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp.proto
--rw-r--r--   0        0        0    56061 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2.py
--rw-r--r--   0        0        0    46909 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2_grpc.py
--rw-r--r--   0        0        0      508 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0001_initial.py
--rw-r--r--   0        0        0     1982 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0002_foreignmodel_manymanymodel_relatedfieldmodel.py
--rw-r--r--   0        0        0      667 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0003_notdisplayedmodel.py
--rw-r--r--   0        0        0      657 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0004_specialfieldsmodel.py
--rw-r--r--   0        0        0      547 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0005_specialfieldsmodel_list_datas.py
--rw-r--r--   0        0        0      631 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0006_specialfieldsmodel_this_is_crazy.py
--rw-r--r--   0        0        0     1104 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0007_auto_20210503_1516.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/__init__.py
--rw-r--r--   0        0        0     4223 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/models.py
--rw-r--r--   0        0        0      386 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/serializers.py
--rw-r--r--   0        0        0      327 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/services/unittestmodel_service.py
--rw-r--r--   0        0        0      433 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/grpc_test_utils/README.md
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/grpc_test_utils/__init__.py
--rw-r--r--   0        0        0     4075 2021-06-29 15:56:50.063511 django-socio-grpc-0.8.9/django_socio_grpc/tests/grpc_test_utils/fake_grpc.py
--rw-r--r--   0        0        0     1577 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_app_handler_registry.py
--rw-r--r--   0        0        0     3402 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_async_model_service.py
--rw-r--r--   0        0        0     3729 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_authentication.py
--rw-r--r--   0        0        0     1745 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_filtering.py
--rw-r--r--   0        0        0     3251 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_model_service.py
--rw-r--r--   0        0        0     2088 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_pagination.py
--rw-r--r--   0        0        0     7707 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_permissions.py
--rw-r--r--   0        0        0     6893 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/test_proto_generation.py
--rw-r--r--   0        0        0     3850 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/tests/utils.py
--rw-r--r--   0        0        0        0 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/utils/__init__.py
--rw-r--r--   0        0        0     1631 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/utils/model_extractor.py
--rw-r--r--   0        0        0      313 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/utils/model_meta.py
--rw-r--r--   0        0        0      970 2021-06-29 15:56:50.067512 django-socio-grpc-0.8.9/django_socio_grpc/utils/servicer_register.py
--rw-r--r--   0        0        0     1012 2021-06-29 15:56:50.103513 django-socio-grpc-0.8.9/pyproject.toml
--rw-r--r--   0        0        0     1349 2021-06-29 15:56:56.224525 django-socio-grpc-0.8.9/setup.py
--rw-r--r--   0        0        0      751 2021-06-29 15:56:56.224929 django-socio-grpc-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/LICENSE
+-rw-r--r--   0        0        0       20 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/__init__.py
+-rw-r--r--   0        0        0      352 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/apps.py
+-rw-r--r--   0        0        0     5268 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/exceptions.py
+-rw-r--r--   0        0        0     9172 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/generics.py
+-rw-r--r--   0        0        0     1334 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/log.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/management/commands/__init__.py
+-rw-r--r--   0        0        0     7169 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/management/commands/generateproto.py
+-rw-r--r--   0        0        0     5110 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/management/commands/grpcrunaioserver.py
+-rw-r--r--   0        0        0     5314 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/management/commands/grpcrunserver.py
+-rw-r--r--   0        0        0    12278 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/mixins.py
+-rw-r--r--   0        0        0     4376 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/proto_serializers.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/protobuf/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/protobuf/default_generated_data.py
+-rw-r--r--   0        0        0    11086 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/protobuf/generators.py
+-rw-r--r--   0        0        0      420 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/protobuf/json_format.py
+-rw-r--r--   0        0        0       97 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/request_transformer/__init_.py
+-rw-r--r--   0        0        0     2535 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/request_transformer/grpc_socio_proxy_context.py
+-rw-r--r--   0        0        0     4151 2021-07-08 16:51:35.967815 django-socio-grpc-0.9.0/django_socio_grpc/servicer_proxy.py
+-rw-r--r--   0        0        0     3136 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/services.py
+-rw-r--r--   0        0        0     4823 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/settings.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/__init__.py
+-rw-r--r--   0        0        0     7886 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/assets/generated_protobuf_files.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/__init__.py
+-rw-r--r--   0        0        0      146 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/apps.py
+-rw-r--r--   0        0        0     4005 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp.proto
+-rw-r--r--   0        0        0    56061 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2.py
+-rw-r--r--   0        0        0    46909 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2_grpc.py
+-rw-r--r--   0        0        0      508 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1982 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0002_foreignmodel_manymanymodel_relatedfieldmodel.py
+-rw-r--r--   0        0        0      667 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0003_notdisplayedmodel.py
+-rw-r--r--   0        0        0      657 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0004_specialfieldsmodel.py
+-rw-r--r--   0        0        0      547 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0005_specialfieldsmodel_list_datas.py
+-rw-r--r--   0        0        0      631 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0006_specialfieldsmodel_this_is_crazy.py
+-rw-r--r--   0        0        0     1104 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0007_auto_20210503_1516.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/__init__.py
+-rw-r--r--   0        0        0     4223 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/models.py
+-rw-r--r--   0        0        0      386 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/serializers.py
+-rw-r--r--   0        0        0      327 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/services/unittestmodel_service.py
+-rw-r--r--   0        0        0      433 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/grpc_test_utils/README.md
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/grpc_test_utils/__init__.py
+-rw-r--r--   0        0        0     4440 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/grpc_test_utils/fake_grpc.py
+-rw-r--r--   0        0        0     1577 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_app_handler_registry.py
+-rw-r--r--   0        0        0     3486 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_async_model_service.py
+-rw-r--r--   0        0        0     3729 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_authentication.py
+-rw-r--r--   0        0        0     1745 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_filtering.py
+-rw-r--r--   0        0        0     3251 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_model_service.py
+-rw-r--r--   0        0        0     2088 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_pagination.py
+-rw-r--r--   0        0        0     7707 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_permissions.py
+-rw-r--r--   0        0        0     7378 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/test_proto_generation.py
+-rw-r--r--   0        0        0     3850 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/tests/utils.py
+-rw-r--r--   0        0        0        0 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/utils/__init__.py
+-rw-r--r--   0        0        0     1631 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/utils/model_extractor.py
+-rw-r--r--   0        0        0      313 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/utils/model_meta.py
+-rw-r--r--   0        0        0      970 2021-07-08 16:51:35.971815 django-socio-grpc-0.9.0/django_socio_grpc/utils/servicer_register.py
+-rw-r--r--   0        0        0     1012 2021-07-08 16:51:36.015815 django-socio-grpc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1349 2021-07-08 16:51:43.063930 django-socio-grpc-0.9.0/setup.py
+-rw-r--r--   0        0        0      751 2021-07-08 16:51:43.064393 django-socio-grpc-0.9.0/PKG-INFO
```

### Comparing `django-socio-grpc-0.8.9/LICENSE` & `django-socio-grpc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/exceptions.py` & `django-socio-grpc-0.9.0/django_socio_grpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/generics.py` & `django-socio-grpc-0.9.0/django_socio_grpc/generics.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/management/commands/generateproto.py` & `django-socio-grpc-0.9.0/django_socio_grpc/management/commands/generateproto.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,18 +105,19 @@
         """
         if self.check and not os.path.exists(file_path):
             raise ProtobufGenerationException(
                 app_name=self.app_name,
                 model_name=self.model_name,
                 detail="Check fail ! You doesn't have a proto file to compare to",
             )
-        with open(file_path, "r+") as f:
-            if self.check:
+        if self.check:
+            with open(file_path, "r+") as f:
                 self.check_proto_generation(f.read(), proto)
-            else:
+        else:
+            with open(file_path, "w+") as f:
                 f.write(proto)
 
     def check_proto_generation(self, original_file, new_proto_content):
         """
         If option --check activated allow to verify that the new generated content is identical to the content of the actual file
         If not raise a ProtobufGenerationException
         """
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/management/commands/grpcrunaioserver.py` & `django-socio-grpc-0.9.0/django_socio_grpc/management/commands/grpcrunaioserver.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/management/commands/grpcrunserver.py` & `django-socio-grpc-0.9.0/django_socio_grpc/management/commands/grpcrunserver.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/mixins.py` & `django-socio-grpc-0.9.0/django_socio_grpc/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,15 @@
 
         .. note::
 
             This is a server streaming RPC.
         """
         messages = await self._get_list_data()
         for message in messages:
-            context.write(message)
+            await context.write(message)
 
 
 class AsyncRetrieveModelMixin(RetrieveModelMixin):
     async def Retrieve(self, request, context):
         async_parent_method = sync_to_async(super().Retrieve)
         return await async_parent_method(request, context)
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/proto_serializers.py` & `django-socio-grpc-0.9.0/django_socio_grpc/proto_serializers.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/protobuf/generators.py` & `django-socio-grpc-0.9.0/django_socio_grpc/protobuf/generators.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/request_transformer/grpc_socio_proxy_context.py` & `django-socio-grpc-0.9.0/django_socio_grpc/request_transformer/grpc_socio_proxy_context.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/servicer_proxy.py` & `django-socio-grpc-0.9.0/django_socio_grpc/servicer_proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     def call_handler(self, action):
         service_instance = self.create_service()
         if self.grpc_async:
 
             async def async_handler(request, context):
                 # db connection state managed similarly to the wsgi handler
                 db.reset_queries()
-                # INFO - AM - 22/04/2021 - next line break tests. Need to more understand the drowback about memory in production
-                # db.close_old_connections()
+                # INFO - AM - 30/06/2021 - Need this in production environnement to avoid SSL end of files errors when too much connection on database
+                await sync_to_async(close_old_connections)()
                 try:
                     service_instance.request = request
                     service_instance.context = GRPCSocioProxyContext(context, action)
                     service_instance.action = action
                     await sync_to_async(service_instance.before_action)()
 
                     # INFO - AM - 05/05/2021 - getting the real function in the service and then calling it if necessary
@@ -40,26 +40,26 @@
                     return await instance_action(
                         service_instance.request, service_instance.context
                     )
                 except GRPCException as grpc_error:
                     logger.error(grpc_error)
                     await context.abort(grpc_error.status_code, grpc_error.get_full_details())
                 finally:
-                    # INFO - AM - 22/04/2021 - next line break tests. Need to more understand the drowback about memory in production
-                    # db.close_old_connections()
+                    # INFO - AM - 30/06/2021 - Need this in production environnement to avoid SSL end of files errors when too much connection on database
+                    await sync_to_async(close_old_connections)()
                     pass
 
             return async_handler
         else:
 
             def handler(request, context):
                 # db connection state managed similarly to the wsgi handler
                 db.reset_queries()
-                # INFO - AM - 22/04/2021 - next line break tests. Need to more understand the drowback about memory in production
-                # db.close_old_connections()
+                # INFO - AM - 30/06/2021 - Need this in production environnement to avoid SSL end of files errors when too much connection on database
+                close_old_connections()
                 try:
                     service_instance.request = request
                     service_instance.context = GRPCSocioProxyContext(context, action)
                     service_instance.action = action
                     service_instance.before_action()
 
                     # INFO - AM - 05/05/2021 - getting the real function in the service and then calling it if necessary
@@ -67,21 +67,27 @@
                     if asyncio.iscoroutinefunction(instance_action):
                         instance_action = async_to_sync(instance_action)
                     return instance_action(service_instance.request, service_instance.context)
                 except GRPCException as grpc_error:
                     logger.error(grpc_error)
                     context.abort(grpc_error.status_code, grpc_error.get_full_details())
                 finally:
-                    # INFO - AM - 22/04/2021 - next line break tests. Need to more understand the drowback about memory in production
-                    # db.close_old_connections()
+                    # INFO - AM - 30/06/2021 - Need this in production environnement to avoid SSL end of files errors when too much connection on database
+                    close_old_connections()
                     pass
 
             return handler
 
     def create_service(self):
         return self.service_class(**self.initkwargs)
 
     def __getattr__(self, action):
         if not hasattr(self.service_class, action):
             raise Unimplemented()
 
         return self.call_handler(action)
+
+
+def close_old_connections():
+    for conn in db.connections.all():
+        if conn.get_autocommit():
+            conn.close_if_unusable_or_obsolete()
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/services.py` & `django-socio-grpc-0.9.0/django_socio_grpc/services.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/settings.py` & `django-socio-grpc-0.9.0/django_socio_grpc/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,27 @@
     "DEFAULT_PAGINATION_CLASS": None,
     #  Default permission classes
     "DEFAULT_PERMISSION_CLASSES": [],
     # gRPC running mode
     "GRPC_ASYNC": False,
     #  Default grpc channel port
     "GRPC_CHANNEL_PORT": 50051,
+    # Default logging action
+    "LOGGING_ACTION": None,
 }
 
 
 # List of settings that may be in string import notation.
 IMPORT_STRINGS = [
     "ROOT_HANDLERS_HOOK",
     "SERVER_INTERCEPTORS",
     "DEFAULT_AUTHENTICATION_CLASSES",
     "DEFAULT_PERMISSION_CLASSES",
     "DEFAULT_PAGINATION_CLASS",
+    "LOGGING_ACTION",
 ]
 
 
 def perform_import(val, setting_name):
     """
     If the given setting is a string import notation,
     then perform the necessary import or imports.
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/assets/generated_protobuf_files.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/assets/generated_protobuf_files.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp.proto` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp.proto`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2_grpc.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/grpc/fakeapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0002_foreignmodel_manymanymodel_relatedfieldmodel.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0002_foreignmodel_manymanymodel_relatedfieldmodel.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0003_notdisplayedmodel.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0003_notdisplayedmodel.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0004_specialfieldsmodel.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0004_specialfieldsmodel.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0005_specialfieldsmodel_list_datas.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0005_specialfieldsmodel_list_datas.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0006_specialfieldsmodel_this_is_crazy.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0006_specialfieldsmodel_this_is_crazy.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/migrations/0007_auto_20210503_1516.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/migrations/0007_auto_20210503_1516.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/fakeapp/models.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/fakeapp/models.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/grpc_test_utils/fake_grpc.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/grpc_test_utils/fake_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # this file is inspirated by pytest-grpc to be able to use django TestCase
 # https://github.com/kataev/pytest-grpc/blob/master/pytest_grpc/plugin.py
 """
 import asyncio
 import socket
 
 import grpc
-from asgiref.sync import async_to_sync
+from asgiref.sync import async_to_sync, sync_to_async
 from grpc._cython.cygrpc import _Metadatum
 
 
 class FakeServer(object):
     def __init__(self):
         self.handlers = {}
 
@@ -61,14 +61,25 @@
         self.stream_pipe.append(data)
 
     def read(self):
         for data in self.stream_pipe:
             yield data
 
 
+class FakeAsyncContext(FakeContext):
+    async def abort(self, code, details):
+        await sync_to_async(super().abort)(code, details)
+
+    async def write(self, data):
+        await sync_to_async(super().write)(data)
+
+    async def read(self):
+        return await sync_to_async(super().read)()
+
+
 def get_brand_new_default_event_loop():
     try:
         old_loop = asyncio.get_event_loop()
         if not old_loop.is_closed():
             old_loop.close()
     except RuntimeError:
         # no default event loop, ignore exception
@@ -99,14 +110,15 @@
             if metadata:
                 self.context._invocation_metadata.extend(
                     (_Metadatum(k, v) for k, v in metadata)
                 )
 
             if asyncio.iscoroutinefunction(real_method):
                 real_method = async_to_sync(real_method)
+                self.context = FakeAsyncContext()
 
             return real_method(request, self.context)
 
         return fake_handler
 
     def unary_unary(self, *args, **kwargs):
         return self.fake_method("unary_unary", *args, **kwargs)
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_app_handler_registry.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_app_handler_registry.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_async_model_service.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_async_model_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from asgiref.sync import async_to_sync
 from django.test import TestCase
 
 from django_socio_grpc import generics, mixins
 from fakeapp.grpc import fakeapp_pb2
 from fakeapp.grpc.fakeapp_pb2_grpc import (
     UnitTestModelControllerStub,
     add_UnitTestModelControllerServicer_to_server,
@@ -82,10 +83,11 @@
         self.assertFalse(UnitTestModel.objects.filter(id=unit_id).exists())
 
     def test_async_stream(self):
         grpc_stub = self.fake_grpc.get_fake_stub(UnitTestModelControllerStub)
         request = fakeapp_pb2.UnitTestModelStreamRequest()
         grpc_stub.Stream(request=request)
 
-        response_list = [response for response in self.fake_grpc.grpc_channel.context.read()]
+        responses = async_to_sync(self.fake_grpc.grpc_channel.context.read)()
+        response_list = [response for response in responses]
 
         self.assertEqual(len(response_list), 10)
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_authentication.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_filtering.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_model_service.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_pagination.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_permissions.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/test_proto_generation.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/test_proto_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,31 @@
             "model": "unittestmodel",
             "file": "proto/unittestmodel.proto",
             "generate_python": False,
         }
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
-        m.assert_called_once_with("proto/unittestmodel.proto", "r+")
+        m.assert_called_once_with("proto/unittestmodel.proto", "w+")
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, SIMPLE_MODEL_GENERATED)
 
+    def test_check_option(self):
+        self.maxDiff = None
+        args = []
+        opts = {"app": "fakeapp", "generate_python": False, "check": True}
+        with patch("builtins.open", mock_open(read_data=ALL_APP_GENERATED)) as m:
+            call_command("generateproto", *args, **opts)
+
+        # this is done to avoid error on different absolute path
+        assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
+        assert m.mock_calls[0].args[1] == "r+"
+
     def test_raise_when_no_app_and_no_model_options(self):
         args = []
         opts = {}
         with self.assertRaises(ProtobufGenerationException) as fake_generation_error:
             call_command("generateproto", *args, **opts)
 
         self.assertEqual(
@@ -86,15 +97,15 @@
         args = []
         opts = {"app": "fakeapp", "model": "RelatedFieldModel", "generate_python": False}
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
 
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, MODEL_WITH_M2M_GENERATED)
 
     def test_generate_one_app_one_model_no_message_no_methods(self):
@@ -103,30 +114,30 @@
         args = []
         opts = {"app": "fakeapp", "model": "NotDisplayedModel", "generate_python": False}
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, SIMPLE_APP_MODEL_NO_GENERATION)
 
     def test_generate_one_app_one_model(self):
         self.maxDiff = None
         args = []
         opts = {"app": "fakeapp", "model": "unittestmodel", "generate_python": False}
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
 
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, SIMPLE_APP_MODEL_GENERATED)
 
     def test_generate_one_app_all_models(self):
@@ -135,15 +146,15 @@
         args = []
         opts = {"app": "fakeapp", "generate_python": False}
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
 
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, ALL_APP_GENERATED)
 
     def test_generate_one_app_one_model_customized(self):
@@ -151,15 +162,15 @@
         args = []
         opts = {"app": "fakeapp", "model": "ForeignModel", "generate_python": False}
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
 
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, CUSTOM_APP_MODEL_GENERATED)
 
     def test_generate_one_app_one_model_import_struct_in_array(self):
@@ -171,13 +182,13 @@
             "generate_python": False,
         }
         with patch("builtins.open", mock_open()) as m:
             call_command("generateproto", *args, **opts)
 
         # this is done to avoid error on different absolute path
         assert m.mock_calls[0].args[0].endswith("fakeapp/grpc/fakeapp.proto")
-        assert m.mock_calls[0].args[1] == "r+"
+        assert m.mock_calls[0].args[1] == "w+"
 
         handle = m()
 
         called_with_data = handle.write.call_args[0][0]
         self.assertEqual(called_with_data, MODEL_WITH_STRUCT_IMORT_IN_ARRAY)
```

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/tests/utils.py` & `django-socio-grpc-0.9.0/django_socio_grpc/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/utils/model_extractor.py` & `django-socio-grpc-0.9.0/django_socio_grpc/utils/model_extractor.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/django_socio_grpc/utils/servicer_register.py` & `django-socio-grpc-0.9.0/django_socio_grpc/utils/servicer_register.py`

 * *Files identical despite different names*

### Comparing `django-socio-grpc-0.8.9/pyproject.toml` & `django-socio-grpc-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-socio-grpc"
-version = "0.8.9"
+version = "0.9.0"
 description = "Fork of django-grpc-framework with more feature maintained by the socio team. Make GRPC with django easy."
 authors = ["Adrien Montagu <adrienmontagu@gmail.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.6"
 django = ">=2.2, <4.0"
```

### Comparing `django-socio-grpc-0.8.9/setup.py` & `django-socio-grpc-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'grpcio-tools']
 
 entry_points = \
 {'console_scripts': ['tests = test_utils.load_tests:launch']}
 
 setup_kwargs = {
     'name': 'django-socio-grpc',
-    'version': '0.8.9',
+    'version': '0.9.0',
     'description': 'Fork of django-grpc-framework with more feature maintained by the socio team. Make GRPC with django easy.',
     'long_description': None,
     'author': 'Adrien Montagu',
     'author_email': 'adrienmontagu@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `django-socio-grpc-0.8.9/PKG-INFO` & `django-socio-grpc-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-socio-grpc
-Version: 0.8.9
+Version: 0.9.0
 Summary: Fork of django-grpc-framework with more feature maintained by the socio team. Make GRPC with django easy.
 License: Apache-2.0
 Author: Adrien Montagu
 Author-email: adrienmontagu@gmail.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

