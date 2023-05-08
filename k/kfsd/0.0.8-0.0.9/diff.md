# Comparing `tmp/kfsd-0.0.8.tar.gz` & `tmp/kfsd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfsd-0.0.8.tar", last modified: Mon May  1 00:17:11 2023, max compression
+gzip compressed data, was "kfsd-0.0.9.tar", last modified: Mon May  1 02:53:48 2023, max compression
```

## Comparing `kfsd-0.0.8.tar` & `kfsd-0.0.9.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 00:16:14.000000 kfsd-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 00:17:11.258560 kfsd-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 00:16:14.000000 kfsd-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.230560 kfsd-0.0.8/kfsd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.230560 kfsd-0.0.8/kfsd/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.230560 kfsd-0.0.8/kfsd/apps/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.234560 kfsd-0.0.8/kfsd/apps/core/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.234560 kfsd-0.0.8/kfsd/apps/core/auth/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/api/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/api/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/api/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.234560 kfsd-0.0.8/kfsd/apps/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/common/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/common/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.234560 kfsd-0.0.8/kfsd/apps/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/exceptions/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/exceptions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/exceptions/fe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.234560 kfsd-0.0.8/kfsd/apps/core/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/middleware/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/middleware/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/middleware/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/base_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/tests/v1/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/tests/v1/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.238560 kfsd-0.0.8/kfsd/apps/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.242560 kfsd-0.0.8/kfsd/apps/core/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.242560 kfsd-0.0.8/kfsd/apps/core/utils/http/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/django/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/django/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/django/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.242560 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/apikey.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/contenttype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/headers/csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/http/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/core/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.242560 kfsd-0.0.8/kfsd/apps/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.242560 kfsd-0.0.8/kfsd/apps/endpoints/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.246560 kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.246560 kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.246560 kfsd-0.0.8/kfsd/apps/endpoints/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/renderers/kubefacetsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/renderers/kubefacetstext.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/renderers/kubefacetsyaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.246560 kfsd-0.0.8/kfsd/apps/endpoints/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.246560 kfsd-0.0.8/kfsd/apps/endpoints/serializers/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/common/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/common/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/arr.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/endpoints_test_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.250560 kfsd-0.0.8/kfsd/apps/endpoints/views/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/common/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/endpoints/views/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/pagination/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/endpoints/views/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/endpoints/views/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/frontend/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.254560 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/browser.html
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/skeleton.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/templates/v1/errors/500.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/tests/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/tests/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/tests/v1/test_api_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/views/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/docs/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/frontend/views/errors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/errors/custom403.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/errors/custom404.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/frontend/views/errors/custom500.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.258560 kfsd-0.0.8/kfsd/apps/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/models/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/apps/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 00:16:14.000000 kfsd-0.0.8/kfsd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 00:17:11.230560 kfsd-0.0.8/kfsd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 00:17:11.000000 kfsd-0.0.8/kfsd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-01 00:17:11.000000 kfsd-0.0.8/kfsd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 00:17:11.000000 kfsd-0.0.8/kfsd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 00:17:11.000000 kfsd-0.0.8/kfsd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 00:17:11.000000 kfsd-0.0.8/kfsd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 00:17:11.258560 kfsd-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 00:16:14.000000 kfsd-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.098708 kfsd-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 02:52:57.000000 kfsd-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 02:53:48.098708 kfsd-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-01 02:52:57.000000 kfsd-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.054707 kfsd-0.0.9/kfsd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.058708 kfsd-0.0.9/kfsd/apps/core/auth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/api/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/common/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/exceptions/fe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/middleware/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/base_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.062708 kfsd-0.0.9/kfsd/apps/core/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.066707 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.070707 kfsd-0.0.9/kfsd/apps/core/utils/http/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/django/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/contenttype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/headers/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/core/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.074707 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetstext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsyaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/common/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.078708 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/endpoints_test_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.082708 kfsd-0.0.9/kfsd/apps/endpoints/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/common/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/pagination/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.086707 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/endpoints/views/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.090707 kfsd-0.0.9/kfsd/apps/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/browser.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/skeleton.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/templates/v1/errors/500.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/tests/v1/test_api_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/docs/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.094708 kfsd-0.0.9/kfsd/apps/frontend/views/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom403.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom404.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/frontend/views/errors/custom500.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.098708 kfsd-0.0.9/kfsd/apps/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/apps/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-01 02:52:57.000000 kfsd-0.0.9/kfsd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 02:53:48.054707 kfsd-0.0.9/kfsd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-01 02:53:48.000000 kfsd-0.0.9/kfsd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 02:53:48.098708 kfsd-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-01 02:52:57.000000 kfsd-0.0.9/setup.py
```

### Comparing `kfsd-0.0.8/kfsd/apps/core/auth/api/gateway.py` & `kfsd-0.0.9/kfsd/apps/core/auth/api/gateway.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/auth/api/token.py` & `kfsd-0.0.9/kfsd/apps/core/auth/api/token.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/common/configuration.py` & `kfsd-0.0.9/kfsd/apps/core/common/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/common/logger.py` & `kfsd-0.0.9/kfsd/apps/core/common/logger.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/common/yaml.py` & `kfsd-0.0.9/kfsd/apps/core/common/yaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/exceptions/api.py` & `kfsd-0.0.9/kfsd/apps/core/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/middleware/config.py` & `kfsd-0.0.9/kfsd/apps/core/middleware/config.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/base_api.py` & `kfsd-0.0.9/kfsd/apps/core/tests/base_api.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_configuration.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_logger.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/common/test_yaml.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/common/test_yaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_arr.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_attr.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_dict.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_dict.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_file.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_file.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/tests/v1/utils/test_system.py` & `kfsd-0.0.9/kfsd/apps/core/tests/v1/utils/test_system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/arr.py` & `kfsd-0.0.9/kfsd/apps/core/utils/arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/attr.py` & `kfsd-0.0.9/kfsd/apps/core/utils/attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/dict.py` & `kfsd-0.0.9/kfsd/apps/core/utils/dict.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/file.py` & `kfsd-0.0.9/kfsd/apps/core/utils/file.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/base.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from kfsd.apps.core.utils.http.response import Response
 
 
 class HTTP(Response):
     def formatUrl(self, args):
         return "/".join(args)
 
-    def genUrlEncode(urlstr):
+    def genUrlEncode(self, urlstr):
         return urllib.parse.quote(urlstr)
 
     def request(self, method, url, expStatus, **kwargs):
         try:
             resp = method(url, **kwargs)
             self.setResponse(resp)
             if self.isRespValid(expStatus):
```

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/django/cookie.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/django/cookie.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/django/request.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/django/request.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/headers/base.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/headers/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/headers/cookie.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/headers/cookie.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/request.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/request.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/http/response.py` & `kfsd-0.0.9/kfsd/apps/core/utils/http/response.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/core/utils/system.py` & `kfsd-0.0.9/kfsd/apps/core/utils/system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/base.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/handlers/common/configuration.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/common/configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/arr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/attr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/handlers/utils/system.py` & `kfsd-0.0.9/kfsd/apps/endpoints/handlers/utils/system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/renderers/kubefacetsjson.py` & `kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsjson.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/renderers/kubefacetsyaml.py` & `kfsd-0.0.9/kfsd/apps/endpoints/renderers/kubefacetsyaml.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/serializers/base.py` & `kfsd-0.0.9/kfsd/apps/endpoints/serializers/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/serializers/utils/system.py` & `kfsd-0.0.9/kfsd/apps/endpoints/serializers/utils/system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/tests/endpoints_test_handler.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/endpoints_test_handler.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/common/test_common_configuration.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_arr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_attr.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py` & `kfsd-0.0.9/kfsd/apps/endpoints/tests/v1/utils/test_utils_system.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/urls.py` & `kfsd-0.0.9/kfsd/apps/endpoints/urls.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/common/list.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/common/list.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/common/serializer.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/common/serializer.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/docs/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/common.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/docs/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/common.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/docs/v1/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/docs/v1/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/utils/common.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/utils/common.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/endpoints/views/utils/utils.py` & `kfsd-0.0.9/kfsd/apps/endpoints/views/utils/utils.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/frontend/templates/v1/base.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/base.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/browser.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/browser.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/frontend/templates/v1/docs/skeleton.html` & `kfsd-0.0.9/kfsd/apps/frontend/templates/v1/docs/skeleton.html`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/apps/models/base.py` & `kfsd-0.0.9/kfsd/apps/models/base.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd/settings.py` & `kfsd-0.0.9/kfsd/settings.py`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/kfsd.egg-info/SOURCES.txt` & `kfsd-0.0.9/kfsd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfsd-0.0.8/setup.py` & `kfsd-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='kfsd',
-    version='0.0.8',
+    version='0.0.9',
     description='Sample App',
     long_description='Sample Pkg',
     long_description_content_type="text/markdown",
     author='Gokul Nathan',
     author_email='nathangokul111@gmail.com',
     packages=find_packages(),
     include_package_data=True,
```

