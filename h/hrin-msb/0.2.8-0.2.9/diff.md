# Comparing `tmp/hrin_msb-0.2.8.tar.gz` & `tmp/hrin_msb-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrin_msb-0.2.8.tar", max compression
+gzip compressed data, was "hrin_msb-0.2.9.tar", max compression
```

## Comparing `hrin_msb-0.2.8.tar` & `hrin_msb-0.2.9.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     1092 2022-11-10 09:38:13.921857 hrin_msb-0.2.8/LICENSE
--rw-r--r--   0        0        0        2 2022-11-10 12:43:54.445000 hrin_msb-0.2.8/msb_apis/__init__.py
--rw-r--r--   0        0        0       40 2022-11-10 11:17:06.989000 hrin_msb-0.2.8/msb_apis/services/__init__.py
--rw-r--r--   0        0        0     1029 2022-12-07 19:03:28.340580 hrin_msb-0.2.8/msb_apis/services/_exceptions.py
--rw-r--r--   0        0        0     3111 2023-03-13 09:53:02.720486 hrin_msb-0.2.8/msb_apis/services/api_services.py
--rw-r--r--   0        0        0      188 2023-02-10 17:26:36.415902 hrin_msb-0.2.8/msb_apis/views/__init__.py
--rw-r--r--   0        0        0     1946 2023-03-13 09:25:43.917431 hrin_msb-0.2.8/msb_apis/views/_api_view.py
--rw-r--r--   0        0        0     5905 2023-03-14 09:04:19.508866 hrin_msb-0.2.8/msb_apis/views/_api_viewset.py
--rw-r--r--   0        0        0     1456 2023-03-04 14:46:50.717490 hrin_msb-0.2.8/msb_apis/views/_constants.py
--rw-r--r--   0        0        0      973 2022-12-07 06:59:33.253000 hrin_msb-0.2.8/msb_apis/views/_errors.py
--rw-r--r--   0        0        0      736 2022-12-09 05:28:51.263454 hrin_msb-0.2.8/msb_apis/views/_exceptions.py
--rw-r--r--   0        0        0      183 2023-02-11 17:31:28.341440 hrin_msb-0.2.8/msb_apis/views/_view.py
--rw-r--r--   0        0        0      234 2023-02-11 17:08:46.861530 hrin_msb-0.2.8/msb_auth/__init__.py
--rw-r--r--   0        0        0     1292 2023-02-12 02:06:52.299167 hrin_msb-0.2.8/msb_auth/_constants.py
--rw-r--r--   0        0        0     2828 2023-02-10 15:14:40.575484 hrin_msb-0.2.8/msb_auth/_defaults.py
--rw-r--r--   0        0        0       75 2023-02-10 15:14:40.593500 hrin_msb-0.2.8/msb_auth/permissions/__init__.py
--rw-r--r--   0        0        0      519 2023-02-10 15:14:40.603008 hrin_msb-0.2.8/msb_auth/permissions/_base_permission.py
--rw-r--r--   0        0        0      769 2023-02-10 15:14:40.612271 hrin_msb-0.2.8/msb_auth/results.py
--rw-r--r--   0        0        0      223 2023-02-11 17:08:46.851570 hrin_msb-0.2.8/msb_auth/users/__init__.py
--rw-r--r--   0        0        0     1755 2023-02-11 17:08:46.885320 hrin_msb-0.2.8/msb_auth/users/_auth_token.py
--rw-r--r--   0        0        0      519 2023-02-10 15:14:40.631191 hrin_msb-0.2.8/msb_auth/users/_datastructures.py
--rw-r--r--   0        0        0     1270 2023-02-10 15:14:40.635549 hrin_msb-0.2.8/msb_auth/users/_token_user.py
--rw-r--r--   0        0        0       52 2023-02-10 15:14:40.641073 hrin_msb-0.2.8/msb_auth/validators/__init__.py
--rw-r--r--   0        0        0     1125 2023-02-10 15:14:40.645182 hrin_msb-0.2.8/msb_auth/validators/jwt_token_validator.py
--rw-r--r--   0        0        0      126 2023-02-10 17:26:36.471242 hrin_msb-0.2.8/msb_cipher/__init__.py
--rw-r--r--   0        0        0       40 2023-01-17 10:59:15.812138 hrin_msb-0.2.8/msb_cipher/_asymmetric_cipher.py
--rw-r--r--   0        0        0        0 2023-01-17 10:56:12.278079 hrin_msb-0.2.8/msb_cipher/_constants.py
--rw-r--r--   0        0        0      160 2023-01-17 11:05:09.496048 hrin_msb-0.2.8/msb_cipher/_exceptions.py
--rw-r--r--   0        0        0      712 2023-02-10 17:26:36.404709 hrin_msb-0.2.8/msb_cipher/_symmetric_cipher.py
--rw-r--r--   0        0        0     1095 2023-02-10 17:26:36.167302 hrin_msb-0.2.8/msb_cipher/cipher.py
--rw-r--r--   0        0        0      102 2023-02-10 17:26:36.302955 hrin_msb-0.2.8/msb_config/__init__.py
--rw-r--r--   0        0        0      222 2023-02-10 17:26:36.217757 hrin_msb-0.2.8/msb_config/_constants.py
--rw-r--r--   0        0        0     1441 2023-02-10 17:26:36.448126 hrin_msb-0.2.8/msb_config/_core.py
--rw-r--r--   0        0        0      380 2022-12-16 15:07:23.828654 hrin_msb-0.2.8/msb_config/_exceptions.py
--rw-r--r--   0        0        0     1684 2022-12-07 06:59:03.505322 hrin_msb-0.2.8/msb_config/_var.py
--rw-r--r--   0        0        0     1078 2023-03-01 23:28:59.608011 hrin_msb-0.2.8/msb_config/main.py
--rw-r--r--   0        0        0      167 2023-02-10 19:05:35.800763 hrin_msb-0.2.8/msb_const/__init__.py
--rw-r--r--   0        0        0      992 2023-03-01 23:26:15.764767 hrin_msb-0.2.8/msb_const/names.py
--rw-r--r--   0        0        0     1638 2023-02-12 02:35:40.088594 hrin_msb-0.2.8/msb_const/paths.py
--rw-r--r--   0        0        0      200 2023-02-10 17:00:14.017572 hrin_msb-0.2.8/msb_const/regex.py
--rw-r--r--   0        0        0      278 2023-02-10 17:26:36.292843 hrin_msb-0.2.8/msb_dataclasses/__init__.py
--rw-r--r--   0        0        0     2077 2022-12-07 06:59:03.498282 hrin_msb-0.2.8/msb_dataclasses/_email.py
--rw-r--r--   0        0        0      928 2022-12-07 06:59:03.499079 hrin_msb-0.2.8/msb_dataclasses/_singleton.py
--rw-r--r--   0        0        0      759 2022-12-22 10:46:31.942723 hrin_msb-0.2.8/msb_dataclasses/_wrappers.py
--rw-r--r--   0        0        0     3058 2023-03-14 09:09:15.392571 hrin_msb-0.2.8/msb_dataclasses/search_parameter.py
--rw-r--r--   0        0        0      356 2022-12-07 06:59:03.539003 hrin_msb-0.2.8/msb_datetime/__init__.py
--rw-r--r--   0        0        0      370 2022-12-14 08:56:16.383990 hrin_msb-0.2.8/msb_datetime/_constants.py
--rw-r--r--   0        0        0     2519 2023-02-10 17:26:36.588823 hrin_msb-0.2.8/msb_datetime/_datetime.py
--rw-r--r--   0        0        0      107 2022-12-22 10:51:56.369719 hrin_msb-0.2.8/msb_db/__init__.py
--rw-r--r--   0        0        0      672 2023-03-04 14:51:33.047339 hrin_msb-0.2.8/msb_db/_constants.py
--rw-r--r--   0        0        0     3750 2023-02-10 17:26:36.198174 hrin_msb-0.2.8/msb_db/_routers.py
--rw-r--r--   0        0        0      653 2023-02-10 17:26:36.482580 hrin_msb-0.2.8/msb_db/models/__init__.py
--rw-r--r--   0        0        0     1178 2022-12-07 11:37:03.118588 hrin_msb-0.2.8/msb_db/models/_fields.py
--rw-r--r--   0        0        0      744 2023-02-10 17:26:36.067375 hrin_msb-0.2.8/msb_db/models/_metafields.py
--rw-r--r--   0        0        0     3532 2023-03-14 09:53:19.137081 hrin_msb-0.2.8/msb_db/models/_model.py
--rw-r--r--   0        0        0      960 2023-02-10 17:26:36.558552 hrin_msb-0.2.8/msb_db/models/_model_manager.py
--rw-r--r--   0        0        0     1141 2023-02-10 17:26:36.101739 hrin_msb-0.2.8/msb_db/models/config_model.py
--rw-r--r--   0        0        0     2559 2023-02-10 17:26:36.521206 hrin_msb-0.2.8/msb_db/models/logging_models.py
--rw-r--r--   0        0        0      413 2023-02-11 17:08:46.894398 hrin_msb-0.2.8/msb_devtools/__init__.py
--rw-r--r--   0        0        0      582 2023-02-10 17:11:44.655700 hrin_msb-0.2.8/msb_devtools/_constants.py
--rw-r--r--   0        0        0     4050 2023-02-11 17:08:46.825121 hrin_msb-0.2.8/msb_devtools/_django.py
--rw-r--r--   0        0        0     2078 2023-02-11 17:12:08.156349 hrin_msb-0.2.8/msb_devtools/_dto.py
--rw-r--r--   0        0        0      977 2023-02-11 09:28:41.800808 hrin_msb-0.2.8/msb_devtools/_funcs.py
--rw-r--r--   0        0        0     3259 2023-02-11 09:45:38.752873 hrin_msb-0.2.8/msb_devtools/_tasks.py
--rw-r--r--   0        0        0      103 2022-12-07 06:59:03.517872 hrin_msb-0.2.8/msb_exceptions/__init__.py
--rw-r--r--   0        0        0      958 2022-12-09 08:38:22.198372 hrin_msb-0.2.8/msb_exceptions/_exception.py
--rw-r--r--   0        0        0      243 2022-12-07 06:59:03.519197 hrin_msb-0.2.8/msb_exceptions/_handlers.py
--rw-r--r--   0        0        0      130 2022-12-07 06:59:03.528914 hrin_msb-0.2.8/msb_files/__init__.py
--rw-r--r--   0        0        0     1050 2023-02-10 17:26:36.327884 hrin_msb-0.2.8/msb_files/_csv.py
--rw-r--r--   0        0        0     1396 2023-02-10 17:26:36.314833 hrin_msb-0.2.8/msb_files/_docx.py
--rw-r--r--   0        0        0      332 2023-02-10 17:26:36.089635 hrin_msb-0.2.8/msb_files/_main.py
--rw-r--r--   0        0        0     1064 2023-02-10 17:26:36.037136 hrin_msb-0.2.8/msb_files/_pdf.py
--rw-r--r--   0        0        0      261 2022-12-07 06:59:03.533708 hrin_msb-0.2.8/msb_files/core/__init__.py
--rw-r--r--   0        0        0      949 2023-02-10 17:26:36.341929 hrin_msb-0.2.8/msb_files/core/_base.py
--rw-r--r--   0        0        0      604 2022-12-07 06:59:33.785432 hrin_msb-0.2.8/msb_files/core/_exceptions.py
--rw-r--r--   0        0        0      181 2022-12-07 06:59:03.536239 hrin_msb-0.2.8/msb_files/core/_generated_file.py
--rw-r--r--   0        0        0      198 2022-12-07 06:59:03.537001 hrin_msb-0.2.8/msb_files/core/_messages.py
--rw-r--r--   0        0        0      251 2023-02-11 17:23:55.748778 hrin_msb-0.2.8/msb_http/__init__.py
--rw-r--r--   0        0        0     2274 2023-02-11 17:06:14.573054 hrin_msb-0.2.8/msb_http/_client.py
--rw-r--r--   0        0        0       49 2023-02-11 17:29:26.506776 hrin_msb-0.2.8/msb_http/_constants.py
--rw-r--r--   0        0        0      893 2023-02-11 17:06:14.579051 hrin_msb-0.2.8/msb_http/_endpoint.py
--rw-r--r--   0        0        0     1959 2023-02-11 17:06:14.583112 hrin_msb-0.2.8/msb_http/_host.py
--rw-r--r--   0        0        0     1497 2023-02-11 17:06:14.587308 hrin_msb-0.2.8/msb_http/_request.py
--rw-r--r--   0        0        0     1525 2023-02-11 17:06:15.028992 hrin_msb-0.2.8/msb_http/_request_wrapper.py
--rw-r--r--   0        0        0     2719 2023-02-11 17:29:30.937884 hrin_msb-0.2.8/msb_http/_response.py
--rw-r--r--   0        0        0      172 2022-12-07 06:59:03.507078 hrin_msb-0.2.8/msb_logging/__init__.py
--rw-r--r--   0        0        0     5283 2023-02-10 17:26:36.119256 hrin_msb-0.2.8/msb_logging/_config.py
--rw-r--r--   0        0        0     1440 2022-12-07 06:59:03.508630 hrin_msb-0.2.8/msb_logging/_constants.py
--rw-r--r--   0        0        0      594 2022-12-07 06:59:03.509280 hrin_msb-0.2.8/msb_logging/_handlers.py
--rw-r--r--   0        0        0       27 2023-02-01 11:12:25.337362 hrin_msb-0.2.8/msb_testing/__init__.py
--rw-r--r--   0        0        0      447 2023-02-01 11:32:20.869417 hrin_msb-0.2.8/msb_testing/_constants.py
--rw-r--r--   0        0        0     1984 2023-02-01 11:18:04.612159 hrin_msb-0.2.8/msb_testing/_core.py
--rw-r--r--   0        0        0     4640 2023-02-10 17:26:36.276023 hrin_msb-0.2.8/msb_testing/api_test.py
--rw-r--r--   0        0        0     3665 2023-02-10 17:26:36.573027 hrin_msb-0.2.8/msb_testing/testdata.py
--rw-r--r--   0        0        0      477 2023-02-10 17:26:36.435186 hrin_msb-0.2.8/msb_testing/unit_test.py
--rw-r--r--   0        0        0      552 2023-02-10 17:26:36.458951 hrin_msb-0.2.8/msb_validation/__init__.py
--rw-r--r--   0        0        0     4694 2023-02-11 17:33:20.648161 hrin_msb-0.2.8/msb_validation/_decorators.py
--rw-r--r--   0        0        0     1023 2023-03-13 11:39:18.804251 hrin_msb-0.2.8/msb_validation/_exceptions.py
--rw-r--r--   0        0        0     1061 2023-03-13 11:37:52.468507 hrin_msb-0.2.8/msb_validation/_rules.py
--rw-r--r--   0        0        0     6480 2022-12-31 11:24:42.573587 hrin_msb-0.2.8/msb_validation/_schema.py
--rw-r--r--   0        0        0     1210 2023-03-14 09:04:47.292107 hrin_msb-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6226 2023-03-14 09:53:19.147285 hrin_msb-0.2.8/README.md
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 hrin_msb-0.2.8/setup.py
--rw-r--r--   0        0        0     6959 1970-01-01 00:00:00.000000 hrin_msb-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1092 2022-11-10 09:38:13.921857 hrin_msb-0.2.9/LICENSE
+-rw-r--r--   0        0        0        2 2022-11-10 12:43:54.445000 hrin_msb-0.2.9/msb_apis/__init__.py
+-rw-r--r--   0        0        0       40 2022-11-10 11:17:06.989000 hrin_msb-0.2.9/msb_apis/services/__init__.py
+-rw-r--r--   0        0        0     1029 2022-12-07 19:03:28.340580 hrin_msb-0.2.9/msb_apis/services/_exceptions.py
+-rw-r--r--   0        0        0     3111 2023-03-13 09:53:02.720486 hrin_msb-0.2.9/msb_apis/services/api_services.py
+-rw-r--r--   0        0        0      188 2023-02-10 17:26:36.415902 hrin_msb-0.2.9/msb_apis/views/__init__.py
+-rw-r--r--   0        0        0     1946 2023-03-13 09:25:43.917431 hrin_msb-0.2.9/msb_apis/views/_api_view.py
+-rw-r--r--   0        0        0     5905 2023-03-14 09:04:19.508866 hrin_msb-0.2.9/msb_apis/views/_api_viewset.py
+-rw-r--r--   0        0        0     1456 2023-03-04 14:46:50.717490 hrin_msb-0.2.9/msb_apis/views/_constants.py
+-rw-r--r--   0        0        0      973 2022-12-07 06:59:33.253000 hrin_msb-0.2.9/msb_apis/views/_errors.py
+-rw-r--r--   0        0        0      736 2022-12-09 05:28:51.263454 hrin_msb-0.2.9/msb_apis/views/_exceptions.py
+-rw-r--r--   0        0        0      183 2023-02-11 17:31:28.341440 hrin_msb-0.2.9/msb_apis/views/_view.py
+-rw-r--r--   0        0        0      234 2023-02-11 17:08:46.861530 hrin_msb-0.2.9/msb_auth/__init__.py
+-rw-r--r--   0        0        0     1292 2023-02-12 02:06:52.299167 hrin_msb-0.2.9/msb_auth/_constants.py
+-rw-r--r--   0        0        0     2828 2023-02-10 15:14:40.575484 hrin_msb-0.2.9/msb_auth/_defaults.py
+-rw-r--r--   0        0        0       75 2023-02-10 15:14:40.593500 hrin_msb-0.2.9/msb_auth/permissions/__init__.py
+-rw-r--r--   0        0        0      519 2023-02-10 15:14:40.603008 hrin_msb-0.2.9/msb_auth/permissions/_base_permission.py
+-rw-r--r--   0        0        0      769 2023-02-10 15:14:40.612271 hrin_msb-0.2.9/msb_auth/results.py
+-rw-r--r--   0        0        0      223 2023-02-11 17:08:46.851570 hrin_msb-0.2.9/msb_auth/users/__init__.py
+-rw-r--r--   0        0        0     1755 2023-02-11 17:08:46.885320 hrin_msb-0.2.9/msb_auth/users/_auth_token.py
+-rw-r--r--   0        0        0      519 2023-02-10 15:14:40.631191 hrin_msb-0.2.9/msb_auth/users/_datastructures.py
+-rw-r--r--   0        0        0     1270 2023-02-10 15:14:40.635549 hrin_msb-0.2.9/msb_auth/users/_token_user.py
+-rw-r--r--   0        0        0       52 2023-02-10 15:14:40.641073 hrin_msb-0.2.9/msb_auth/validators/__init__.py
+-rw-r--r--   0        0        0     1125 2023-02-10 15:14:40.645182 hrin_msb-0.2.9/msb_auth/validators/jwt_token_validator.py
+-rw-r--r--   0        0        0      126 2023-02-10 17:26:36.471242 hrin_msb-0.2.9/msb_cipher/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-17 10:59:15.812138 hrin_msb-0.2.9/msb_cipher/_asymmetric_cipher.py
+-rw-r--r--   0        0        0        0 2023-01-17 10:56:12.278079 hrin_msb-0.2.9/msb_cipher/_constants.py
+-rw-r--r--   0        0        0      160 2023-01-17 11:05:09.496048 hrin_msb-0.2.9/msb_cipher/_exceptions.py
+-rw-r--r--   0        0        0      712 2023-02-10 17:26:36.404709 hrin_msb-0.2.9/msb_cipher/_symmetric_cipher.py
+-rw-r--r--   0        0        0     1095 2023-02-10 17:26:36.167302 hrin_msb-0.2.9/msb_cipher/cipher.py
+-rw-r--r--   0        0        0      102 2023-02-10 17:26:36.302955 hrin_msb-0.2.9/msb_config/__init__.py
+-rw-r--r--   0        0        0      222 2023-02-10 17:26:36.217757 hrin_msb-0.2.9/msb_config/_constants.py
+-rw-r--r--   0        0        0     1441 2023-02-10 17:26:36.448126 hrin_msb-0.2.9/msb_config/_core.py
+-rw-r--r--   0        0        0      380 2022-12-16 15:07:23.828654 hrin_msb-0.2.9/msb_config/_exceptions.py
+-rw-r--r--   0        0        0     1684 2022-12-07 06:59:03.505322 hrin_msb-0.2.9/msb_config/_var.py
+-rw-r--r--   0        0        0     1078 2023-03-01 23:28:59.608011 hrin_msb-0.2.9/msb_config/main.py
+-rw-r--r--   0        0        0      167 2023-02-10 19:05:35.800763 hrin_msb-0.2.9/msb_const/__init__.py
+-rw-r--r--   0        0        0      992 2023-03-01 23:26:15.764767 hrin_msb-0.2.9/msb_const/names.py
+-rw-r--r--   0        0        0     1638 2023-02-12 02:35:40.088594 hrin_msb-0.2.9/msb_const/paths.py
+-rw-r--r--   0        0        0      200 2023-02-10 17:00:14.017572 hrin_msb-0.2.9/msb_const/regex.py
+-rw-r--r--   0        0        0      278 2023-02-10 17:26:36.292843 hrin_msb-0.2.9/msb_dataclasses/__init__.py
+-rw-r--r--   0        0        0     2077 2022-12-07 06:59:03.498282 hrin_msb-0.2.9/msb_dataclasses/_email.py
+-rw-r--r--   0        0        0      928 2022-12-07 06:59:03.499079 hrin_msb-0.2.9/msb_dataclasses/_singleton.py
+-rw-r--r--   0        0        0      759 2022-12-22 10:46:31.942723 hrin_msb-0.2.9/msb_dataclasses/_wrappers.py
+-rw-r--r--   0        0        0     3058 2023-03-14 09:09:15.392571 hrin_msb-0.2.9/msb_dataclasses/search_parameter.py
+-rw-r--r--   0        0        0      356 2022-12-07 06:59:03.539003 hrin_msb-0.2.9/msb_datetime/__init__.py
+-rw-r--r--   0        0        0      370 2022-12-14 08:56:16.383990 hrin_msb-0.2.9/msb_datetime/_constants.py
+-rw-r--r--   0        0        0     2519 2023-02-10 17:26:36.588823 hrin_msb-0.2.9/msb_datetime/_datetime.py
+-rw-r--r--   0        0        0      107 2022-12-22 10:51:56.369719 hrin_msb-0.2.9/msb_db/__init__.py
+-rw-r--r--   0        0        0      672 2023-03-04 14:51:33.047339 hrin_msb-0.2.9/msb_db/_constants.py
+-rw-r--r--   0        0        0     3750 2023-02-10 17:26:36.198174 hrin_msb-0.2.9/msb_db/_routers.py
+-rw-r--r--   0        0        0      653 2023-02-10 17:26:36.482580 hrin_msb-0.2.9/msb_db/models/__init__.py
+-rw-r--r--   0        0        0     1178 2022-12-07 11:37:03.118588 hrin_msb-0.2.9/msb_db/models/_fields.py
+-rw-r--r--   0        0        0      744 2023-02-10 17:26:36.067375 hrin_msb-0.2.9/msb_db/models/_metafields.py
+-rw-r--r--   0        0        0     3758 2023-03-14 10:22:15.638183 hrin_msb-0.2.9/msb_db/models/_model.py
+-rw-r--r--   0        0        0      960 2023-02-10 17:26:36.558552 hrin_msb-0.2.9/msb_db/models/_model_manager.py
+-rw-r--r--   0        0        0     1141 2023-02-10 17:26:36.101739 hrin_msb-0.2.9/msb_db/models/config_model.py
+-rw-r--r--   0        0        0     2559 2023-02-10 17:26:36.521206 hrin_msb-0.2.9/msb_db/models/logging_models.py
+-rw-r--r--   0        0        0      413 2023-02-11 17:08:46.894398 hrin_msb-0.2.9/msb_devtools/__init__.py
+-rw-r--r--   0        0        0      582 2023-02-10 17:11:44.655700 hrin_msb-0.2.9/msb_devtools/_constants.py
+-rw-r--r--   0        0        0     4050 2023-02-11 17:08:46.825121 hrin_msb-0.2.9/msb_devtools/_django.py
+-rw-r--r--   0        0        0     2078 2023-02-11 17:12:08.156349 hrin_msb-0.2.9/msb_devtools/_dto.py
+-rw-r--r--   0        0        0      977 2023-02-11 09:28:41.800808 hrin_msb-0.2.9/msb_devtools/_funcs.py
+-rw-r--r--   0        0        0     3259 2023-02-11 09:45:38.752873 hrin_msb-0.2.9/msb_devtools/_tasks.py
+-rw-r--r--   0        0        0      103 2022-12-07 06:59:03.517872 hrin_msb-0.2.9/msb_exceptions/__init__.py
+-rw-r--r--   0        0        0      958 2022-12-09 08:38:22.198372 hrin_msb-0.2.9/msb_exceptions/_exception.py
+-rw-r--r--   0        0        0      243 2022-12-07 06:59:03.519197 hrin_msb-0.2.9/msb_exceptions/_handlers.py
+-rw-r--r--   0        0        0      130 2022-12-07 06:59:03.528914 hrin_msb-0.2.9/msb_files/__init__.py
+-rw-r--r--   0        0        0     1050 2023-02-10 17:26:36.327884 hrin_msb-0.2.9/msb_files/_csv.py
+-rw-r--r--   0        0        0     1396 2023-02-10 17:26:36.314833 hrin_msb-0.2.9/msb_files/_docx.py
+-rw-r--r--   0        0        0      332 2023-02-10 17:26:36.089635 hrin_msb-0.2.9/msb_files/_main.py
+-rw-r--r--   0        0        0     1064 2023-02-10 17:26:36.037136 hrin_msb-0.2.9/msb_files/_pdf.py
+-rw-r--r--   0        0        0      261 2022-12-07 06:59:03.533708 hrin_msb-0.2.9/msb_files/core/__init__.py
+-rw-r--r--   0        0        0      949 2023-02-10 17:26:36.341929 hrin_msb-0.2.9/msb_files/core/_base.py
+-rw-r--r--   0        0        0      604 2022-12-07 06:59:33.785432 hrin_msb-0.2.9/msb_files/core/_exceptions.py
+-rw-r--r--   0        0        0      181 2022-12-07 06:59:03.536239 hrin_msb-0.2.9/msb_files/core/_generated_file.py
+-rw-r--r--   0        0        0      198 2022-12-07 06:59:03.537001 hrin_msb-0.2.9/msb_files/core/_messages.py
+-rw-r--r--   0        0        0      251 2023-02-11 17:23:55.748778 hrin_msb-0.2.9/msb_http/__init__.py
+-rw-r--r--   0        0        0     2274 2023-02-11 17:06:14.573054 hrin_msb-0.2.9/msb_http/_client.py
+-rw-r--r--   0        0        0       49 2023-02-11 17:29:26.506776 hrin_msb-0.2.9/msb_http/_constants.py
+-rw-r--r--   0        0        0      893 2023-02-11 17:06:14.579051 hrin_msb-0.2.9/msb_http/_endpoint.py
+-rw-r--r--   0        0        0     1959 2023-02-11 17:06:14.583112 hrin_msb-0.2.9/msb_http/_host.py
+-rw-r--r--   0        0        0     1497 2023-02-11 17:06:14.587308 hrin_msb-0.2.9/msb_http/_request.py
+-rw-r--r--   0        0        0     1525 2023-02-11 17:06:15.028992 hrin_msb-0.2.9/msb_http/_request_wrapper.py
+-rw-r--r--   0        0        0     2719 2023-02-11 17:29:30.937884 hrin_msb-0.2.9/msb_http/_response.py
+-rw-r--r--   0        0        0      172 2022-12-07 06:59:03.507078 hrin_msb-0.2.9/msb_logging/__init__.py
+-rw-r--r--   0        0        0     5283 2023-02-10 17:26:36.119256 hrin_msb-0.2.9/msb_logging/_config.py
+-rw-r--r--   0        0        0     1440 2022-12-07 06:59:03.508630 hrin_msb-0.2.9/msb_logging/_constants.py
+-rw-r--r--   0        0        0      594 2022-12-07 06:59:03.509280 hrin_msb-0.2.9/msb_logging/_handlers.py
+-rw-r--r--   0        0        0       27 2023-02-01 11:12:25.337362 hrin_msb-0.2.9/msb_testing/__init__.py
+-rw-r--r--   0        0        0      447 2023-02-01 11:32:20.869417 hrin_msb-0.2.9/msb_testing/_constants.py
+-rw-r--r--   0        0        0     1984 2023-02-01 11:18:04.612159 hrin_msb-0.2.9/msb_testing/_core.py
+-rw-r--r--   0        0        0     4640 2023-02-10 17:26:36.276023 hrin_msb-0.2.9/msb_testing/api_test.py
+-rw-r--r--   0        0        0     3665 2023-02-10 17:26:36.573027 hrin_msb-0.2.9/msb_testing/testdata.py
+-rw-r--r--   0        0        0      477 2023-02-10 17:26:36.435186 hrin_msb-0.2.9/msb_testing/unit_test.py
+-rw-r--r--   0        0        0      552 2023-02-10 17:26:36.458951 hrin_msb-0.2.9/msb_validation/__init__.py
+-rw-r--r--   0        0        0     4694 2023-02-11 17:33:20.648161 hrin_msb-0.2.9/msb_validation/_decorators.py
+-rw-r--r--   0        0        0     1023 2023-03-13 11:39:18.804251 hrin_msb-0.2.9/msb_validation/_exceptions.py
+-rw-r--r--   0        0        0     1061 2023-03-13 11:37:52.468507 hrin_msb-0.2.9/msb_validation/_rules.py
+-rw-r--r--   0        0        0     6480 2022-12-31 11:24:42.573587 hrin_msb-0.2.9/msb_validation/_schema.py
+-rw-r--r--   0        0        0     1210 2023-03-14 10:23:02.476193 hrin_msb-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6382 2023-03-14 10:23:26.105369 hrin_msb-0.2.9/README.md
+-rw-r--r--   0        0        0     7705 1970-01-01 00:00:00.000000 hrin_msb-0.2.9/setup.py
+-rw-r--r--   0        0        0     7111 1970-01-01 00:00:00.000000 hrin_msb-0.2.9/PKG-INFO
```

### Comparing `hrin_msb-0.2.8/LICENSE` & `hrin_msb-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/services/_exceptions.py` & `hrin_msb-0.2.9/msb_apis/services/_exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/services/api_services.py` & `hrin_msb-0.2.9/msb_apis/services/api_services.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/views/_api_view.py` & `hrin_msb-0.2.9/msb_apis/views/_api_view.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/views/_api_viewset.py` & `hrin_msb-0.2.9/msb_apis/views/_api_viewset.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/views/_constants.py` & `hrin_msb-0.2.9/msb_apis/views/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/views/_errors.py` & `hrin_msb-0.2.9/msb_apis/views/_errors.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_apis/views/_exceptions.py` & `hrin_msb-0.2.9/msb_apis/views/_exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/_constants.py` & `hrin_msb-0.2.9/msb_auth/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/_defaults.py` & `hrin_msb-0.2.9/msb_auth/_defaults.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/permissions/_base_permission.py` & `hrin_msb-0.2.9/msb_auth/permissions/_base_permission.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/results.py` & `hrin_msb-0.2.9/msb_auth/results.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/users/_auth_token.py` & `hrin_msb-0.2.9/msb_auth/users/_auth_token.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/users/_datastructures.py` & `hrin_msb-0.2.9/msb_auth/users/_datastructures.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/users/_token_user.py` & `hrin_msb-0.2.9/msb_auth/users/_token_user.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_auth/validators/jwt_token_validator.py` & `hrin_msb-0.2.9/msb_auth/validators/jwt_token_validator.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_cipher/_symmetric_cipher.py` & `hrin_msb-0.2.9/msb_cipher/_symmetric_cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_cipher/cipher.py` & `hrin_msb-0.2.9/msb_cipher/cipher.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_config/_core.py` & `hrin_msb-0.2.9/msb_config/_core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_config/_var.py` & `hrin_msb-0.2.9/msb_config/_var.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_config/main.py` & `hrin_msb-0.2.9/msb_config/main.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_const/names.py` & `hrin_msb-0.2.9/msb_const/names.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_const/paths.py` & `hrin_msb-0.2.9/msb_const/paths.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_dataclasses/_email.py` & `hrin_msb-0.2.9/msb_dataclasses/_email.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_dataclasses/_singleton.py` & `hrin_msb-0.2.9/msb_dataclasses/_singleton.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_dataclasses/_wrappers.py` & `hrin_msb-0.2.9/msb_dataclasses/_wrappers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_dataclasses/search_parameter.py` & `hrin_msb-0.2.9/msb_dataclasses/search_parameter.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_datetime/_datetime.py` & `hrin_msb-0.2.9/msb_datetime/_datetime.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/_constants.py` & `hrin_msb-0.2.9/msb_db/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/_routers.py` & `hrin_msb-0.2.9/msb_db/_routers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/__init__.py` & `hrin_msb-0.2.9/msb_db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/_fields.py` & `hrin_msb-0.2.9/msb_db/models/_fields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/_metafields.py` & `hrin_msb-0.2.9/msb_db/models/_metafields.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/_model.py` & `hrin_msb-0.2.9/msb_db/models/_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,33 @@
 
 from msb_cipher import Cipher
 from ._model_manager import MsbModelManager
 from .._constants import (COLUMN_NAME_DELETED, COLUMN_NAME_DELETED_BY)
 from django.conf import settings
 
 DB_ENCRYPT_PRIVATE_FIELDS = getattr(settings, 'DB_ENCRYPT_PRIVATE_FIELDS', False)
+DB_PK_IS_PRIVATE_FIELD = getattr(settings, 'DB_PK_IS_PRIVATE_FIELD', False)
+
 
 class MsbModel(Models.Model):
 	_private_fields: list = []
 	_list_field_names: list = []
 	_identifier_field: str = ""
 	_encrypt_private_fields: bool = DB_ENCRYPT_PRIVATE_FIELDS
+	_pk_is_private_fields: bool = DB_PK_IS_PRIVATE_FIELD
 
 	class Meta:
 		abstract = True
 
 	@property
 	def secure_fields(self):
-		return [self._meta.pk.attname, *self._private_fields]
+		_secure_fields = self._private_fields if isinstance(self._private_fields, list) else []
+		if self._pk_is_private_fields:
+			_secure_fields.append(self._meta.pk.attname)
+		return _secure_fields
 
 	@property
 	def identifier_field_name(self):
 		if isinstance(self._identifier_field, str) and len(self._identifier_field) > 0:
 			return self._identifier_field
 		return ''
 
@@ -37,16 +43,19 @@
 				field_value = getattr(self, field_name, default)
 				if isinstance(field_value, MsbModel):
 					field_value = field_value._get_field_value(field_value.pk_name)
 
 		except Exception as e:
 			field_value = None
 		finally:
-			return Cipher.encrypt(field_value) if (field_name is not None and field_value is not None) \
-			                                      and (field_name in self.secure_fields or encrypt) else field_value
+
+			if (field_name in self.secure_fields) and (encrypt or self._encrypt_private_fields):
+				return Cipher.encrypt(field_value)
+			return field_value
+
 
 	@property
 	def related_fields(self):
 		fields = []
 		for field in self._meta.fields:
 			if field.get_internal_type() in ['ForeignKey']:
 				fields.append(field.name)
```

### Comparing `hrin_msb-0.2.8/msb_db/models/_model_manager.py` & `hrin_msb-0.2.9/msb_db/models/_model_manager.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/config_model.py` & `hrin_msb-0.2.9/msb_db/models/config_model.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_db/models/logging_models.py` & `hrin_msb-0.2.9/msb_db/models/logging_models.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_devtools/_constants.py` & `hrin_msb-0.2.9/msb_devtools/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_devtools/_django.py` & `hrin_msb-0.2.9/msb_devtools/_django.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_devtools/_dto.py` & `hrin_msb-0.2.9/msb_devtools/_dto.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_devtools/_funcs.py` & `hrin_msb-0.2.9/msb_devtools/_funcs.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_devtools/_tasks.py` & `hrin_msb-0.2.9/msb_devtools/_tasks.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_exceptions/_exception.py` & `hrin_msb-0.2.9/msb_exceptions/_exception.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_files/_csv.py` & `hrin_msb-0.2.9/msb_files/_csv.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_files/_docx.py` & `hrin_msb-0.2.9/msb_files/_docx.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_files/_pdf.py` & `hrin_msb-0.2.9/msb_files/_pdf.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_files/core/_base.py` & `hrin_msb-0.2.9/msb_files/core/_base.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_files/core/_exceptions.py` & `hrin_msb-0.2.9/msb_files/core/_exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_client.py` & `hrin_msb-0.2.9/msb_http/_client.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_endpoint.py` & `hrin_msb-0.2.9/msb_http/_endpoint.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_host.py` & `hrin_msb-0.2.9/msb_http/_host.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_request.py` & `hrin_msb-0.2.9/msb_http/_request.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_request_wrapper.py` & `hrin_msb-0.2.9/msb_http/_request_wrapper.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_http/_response.py` & `hrin_msb-0.2.9/msb_http/_response.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_logging/_config.py` & `hrin_msb-0.2.9/msb_logging/_config.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_logging/_constants.py` & `hrin_msb-0.2.9/msb_logging/_constants.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_logging/_handlers.py` & `hrin_msb-0.2.9/msb_logging/_handlers.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_testing/_core.py` & `hrin_msb-0.2.9/msb_testing/_core.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_testing/api_test.py` & `hrin_msb-0.2.9/msb_testing/api_test.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_testing/testdata.py` & `hrin_msb-0.2.9/msb_testing/testdata.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_validation/__init__.py` & `hrin_msb-0.2.9/msb_validation/__init__.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_validation/_decorators.py` & `hrin_msb-0.2.9/msb_validation/_decorators.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_validation/_exceptions.py` & `hrin_msb-0.2.9/msb_validation/_exceptions.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_validation/_rules.py` & `hrin_msb-0.2.9/msb_validation/_rules.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/msb_validation/_schema.py` & `hrin_msb-0.2.9/msb_validation/_schema.py`

 * *Files identical despite different names*

### Comparing `hrin_msb-0.2.8/pyproject.toml` & `hrin_msb-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hrin-msb"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = [
     "Prakash Mishra <prakash.mishra@intimetec.com>",
     "Mohit Verma<mohit.verma@intimetec.com>",
     "Prajwal S <prajwal.s@intimetec.com>",
 ]
 readme = "README.md"
```

### Comparing `hrin_msb-0.2.8/README.md` & `hrin_msb-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -150,8 +150,12 @@
 ### -- Version 0.2.7
 1. Fixed : `_list_field_names` not working with properties & relations 
 2. Added `search_validation_rules` in DefaultRules
 
 ### -- Version 0.2.8
 1. Fixed : list api breaking for foreign keys
 2. Fixed : Search parameter not working with fields
-3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.
+3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.
+
+### -- Version 0.2.9
+1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve 
+   that.
```

### Comparing `hrin_msb-0.2.8/setup.py` & `hrin_msb-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
  'python-dateutil>=2.8.2,<3.0.0',
  'python-dotenv>=0.21.0,<0.22.0',
  'requests>=2.28.1,<3.0.0',
  'xhtml2pdf>=0.2.8,<0.3.0']
 
 setup_kwargs = {
     'name': 'hrin-msb',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': '',
-    'long_description': '# hrin-msb\n\n## Pre-requisites for setup\n1. `pip install poetry`\n\n## How To Build\n\n1. `poetry build`\n2. `poetry config http-basic.pypi __token__ <access-token>`\n3. `poetry publish`\n\n\n# Change Log\n ### Version 0.1.1\n***\n\n ### Version 0.1.2\n***\n\n ### Version 0.1.3\n***\n\n1.  Default serializer added to ApiView\n2. fixed incorrect import in _validators.py\n3. fixed msb_database_router\n4. fixed Config.is_local_env() not working\n5. moved devscripts -> devtools\n6. File Utils Added to utils/files\n7. "app_label" removed from "TestConfig" & "ApiTest" Classes\n8. Fixed Bug : \'LoggingModelManager\' object has no attribute \'_queryset_class\'\n9. Fixed : Logging Model not showing any records\n10. Fixed : str method for base model, & removed current_timestamp method from base model\n***\n\n ## Version 0.1.4\n1. Fixed : ModuleNotFoundError: No module named \'pdf2docx\'\n2. Renamed “FileGenerator“ => “FileFactory”,\n3. Add `create_` Prefix in FileFactory methods\n4. Renamed MsbMetaModel -> MsbModelMetaFields\n5. Added validation decorators, and fixed bulk validation issuses\n6. Modified Logging Configuration Files\n7. removed utils package\n8. moved msb_core.wrappers.exceptions -> msb_exceptions\n9. Fixed : Base ApiViews and Crud Routes\n10. Searchparameter class refactored, search method added in ApiService Class\n***\n\n## Version 0.1.41\n1. Fixed: Crud operations not working with encrypted id\'s\n2. Package dependencies updated\n3. Validator test cases refactored\n***\n## Version 0.1.5x\n ### -- Version 0.1.51\n1. dbrouter print statement removed\n2. datetime constants renamed (added _FORMAT to all fof them)\n3. Fixed the default argument in msb_exception  which was causing "DESC :" to log even if desc was none\n4. Api service create methdhod not working correctly\n5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it \n6. SearchParameter class imported in package.__init__.py \n7. Fixed : test-cases are breaking because of logs databae\n8. added base unittest class, and modified unit_test to inherit djangoTestCase instead of unittest\n9. Added Validation Schema not defined exceptions\n10. Fixed init_django_app error, int datatype instead of str while setting environement variable.\n11. Added use_django decorator to use over classes/functions\n12. Fixed : MsbMetaModel not working\n13. MsbModel meta fields accessor added\n14. Poetry dependencies updated\n15. DMY_DATE_FORMAT added\n16. versioning changed\n\n  ### -- Version 0.1.52\n1. Fixed : MsbMetaFields not working \n2. Fixed : logging model lot of exceptions are thrown if table applicationlogs is not found\n3. Fixed : logging model exceptions file not found\n4. Fixed : db_migration throwing error if no migration dire is found\n5. renamed use_djnago -> use_django, default value for settinfs_dir is added to "app"\n6. renamend _query in msb_model to db_query\n7. field_type, and label added to configuration model\n8. unique_together constraint added to ConfigurationModel\n9. class DjangoMigration creates migration folder if it doesn\'t exists\n10. Added automatic fixture loading\n11. Fixed : msb_model.__str__() was not able to read the primary key value \n12. comma removed from msbMetamodels\n13. Cipher now supports encryption/decryption of list items \n14. SearchParameter modified to supoprt autmatic filter assignment \n15. Refactor `msb_auth` : TokenUser,AuthResult,Constants added\n16. Jwt Token Validation is strict now, it allows only same owner\n  \n### -- Version 0.1.521\n1. Fixed improper import exception\n\n  \n### -- Version 0.1.522\n1. Added Login Required to base viewset\n2. Added Config Object class to msb_dataclasses \n3. Added msb_http to the package\n4. Added MsbDatabaseRouter in init.py\n5. Fixed model.delete() is not working\n\n### -- Version 0.1.611\n1. Modified django migration script\n2. Aded devtools to msb_ext\n3. removed `use_django` decorator & added `requires_django` decorator\n4. added default values for metafields\n5. added InputFiled.time in validation schema types\n\n\n### -- Version 0.2.0\n1. Fixed Cipher.decrypt() returning bytes instead of str\n2. Changed `SearchParameter` class implementation.\n3. default offset & limit fixed in `SearchParameter` class\n\n### -- Version 0.2.2\n1. default values removed from model metafields\n2. Fixed `ModuleNotFoundError: No module named \'_asymmetric_cipher\'`\n3. Fixed fixtures loaded in wrong sequence\n4. Feature `api_response.exception()` now sends back internal server error for undefined exceptions.\n5. Fixed Token validation error\n6. Added `DefaultJwtAuthSettings()` class, to unify settings across the services\n7. Added automatic fixture loading for test cases.\n\n\n### -- Version 0.2.3\n1. msb_testing refactored \n2. added new package `msb_const`\n3. Optimized imports throughout\n4. Refactored `msb_devtools`, removed `msb_ext.devtools`\n5. `msb_devtools._exceptions` file removed\n6. Added constant to `mab_auth._constants`\n\n### -- Version 0.2.4\n1. Refactor : (Optimized Imports,Sonarlint warnings)\n2. Refactor : Moved msb_apis.wrappers -> msb_http\n\n### -- Version 0.2.5\n1. Refactor : removed `msb_ext`, as it served no purpose\n2. Fixed : token validation failing due to AUD & ISS claim\n3. Added default fixture paths to `msb_const.paths`\n\n### -- Version 0.2.6\n1. renamed the property `db_query` to `rows`, to make it easier to understand.\n2. added a mentod to deteremine if the current environment is either dev or test env\n3. CrudActions.all is now the default parameter value for `.as_view()` method.\n4. Crud routes not working for single fields\n5. Fixed `self.seriallizer` not working with `dict()`\n6. Implemented `list` Api, to return predefined db columns \n7. search parameter added in crud, searchparameters class refatored\n\n### -- Version 0.2.7\n1. Fixed : `_list_field_names` not working with properties & relations \n2. Added `search_validation_rules` in DefaultRules\n\n### -- Version 0.2.8\n1. Fixed : list api breaking for foreign keys\n2. Fixed : Search parameter not working with fields\n3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.',
+    'long_description': '# hrin-msb\n\n## Pre-requisites for setup\n1. `pip install poetry`\n\n## How To Build\n\n1. `poetry build`\n2. `poetry config http-basic.pypi __token__ <access-token>`\n3. `poetry publish`\n\n\n# Change Log\n ### Version 0.1.1\n***\n\n ### Version 0.1.2\n***\n\n ### Version 0.1.3\n***\n\n1.  Default serializer added to ApiView\n2. fixed incorrect import in _validators.py\n3. fixed msb_database_router\n4. fixed Config.is_local_env() not working\n5. moved devscripts -> devtools\n6. File Utils Added to utils/files\n7. "app_label" removed from "TestConfig" & "ApiTest" Classes\n8. Fixed Bug : \'LoggingModelManager\' object has no attribute \'_queryset_class\'\n9. Fixed : Logging Model not showing any records\n10. Fixed : str method for base model, & removed current_timestamp method from base model\n***\n\n ## Version 0.1.4\n1. Fixed : ModuleNotFoundError: No module named \'pdf2docx\'\n2. Renamed “FileGenerator“ => “FileFactory”,\n3. Add `create_` Prefix in FileFactory methods\n4. Renamed MsbMetaModel -> MsbModelMetaFields\n5. Added validation decorators, and fixed bulk validation issuses\n6. Modified Logging Configuration Files\n7. removed utils package\n8. moved msb_core.wrappers.exceptions -> msb_exceptions\n9. Fixed : Base ApiViews and Crud Routes\n10. Searchparameter class refactored, search method added in ApiService Class\n***\n\n## Version 0.1.41\n1. Fixed: Crud operations not working with encrypted id\'s\n2. Package dependencies updated\n3. Validator test cases refactored\n***\n## Version 0.1.5x\n ### -- Version 0.1.51\n1. dbrouter print statement removed\n2. datetime constants renamed (added _FORMAT to all fof them)\n3. Fixed the default argument in msb_exception  which was causing "DESC :" to log even if desc was none\n4. Api service create methdhod not working correctly\n5. file logging handler is not registered in local env by default, we need to pass `emulate_prod=True` to add it \n6. SearchParameter class imported in package.__init__.py \n7. Fixed : test-cases are breaking because of logs databae\n8. added base unittest class, and modified unit_test to inherit djangoTestCase instead of unittest\n9. Added Validation Schema not defined exceptions\n10. Fixed init_django_app error, int datatype instead of str while setting environement variable.\n11. Added use_django decorator to use over classes/functions\n12. Fixed : MsbMetaModel not working\n13. MsbModel meta fields accessor added\n14. Poetry dependencies updated\n15. DMY_DATE_FORMAT added\n16. versioning changed\n\n  ### -- Version 0.1.52\n1. Fixed : MsbMetaFields not working \n2. Fixed : logging model lot of exceptions are thrown if table applicationlogs is not found\n3. Fixed : logging model exceptions file not found\n4. Fixed : db_migration throwing error if no migration dire is found\n5. renamed use_djnago -> use_django, default value for settinfs_dir is added to "app"\n6. renamend _query in msb_model to db_query\n7. field_type, and label added to configuration model\n8. unique_together constraint added to ConfigurationModel\n9. class DjangoMigration creates migration folder if it doesn\'t exists\n10. Added automatic fixture loading\n11. Fixed : msb_model.__str__() was not able to read the primary key value \n12. comma removed from msbMetamodels\n13. Cipher now supports encryption/decryption of list items \n14. SearchParameter modified to supoprt autmatic filter assignment \n15. Refactor `msb_auth` : TokenUser,AuthResult,Constants added\n16. Jwt Token Validation is strict now, it allows only same owner\n  \n### -- Version 0.1.521\n1. Fixed improper import exception\n\n  \n### -- Version 0.1.522\n1. Added Login Required to base viewset\n2. Added Config Object class to msb_dataclasses \n3. Added msb_http to the package\n4. Added MsbDatabaseRouter in init.py\n5. Fixed model.delete() is not working\n\n### -- Version 0.1.611\n1. Modified django migration script\n2. Aded devtools to msb_ext\n3. removed `use_django` decorator & added `requires_django` decorator\n4. added default values for metafields\n5. added InputFiled.time in validation schema types\n\n\n### -- Version 0.2.0\n1. Fixed Cipher.decrypt() returning bytes instead of str\n2. Changed `SearchParameter` class implementation.\n3. default offset & limit fixed in `SearchParameter` class\n\n### -- Version 0.2.2\n1. default values removed from model metafields\n2. Fixed `ModuleNotFoundError: No module named \'_asymmetric_cipher\'`\n3. Fixed fixtures loaded in wrong sequence\n4. Feature `api_response.exception()` now sends back internal server error for undefined exceptions.\n5. Fixed Token validation error\n6. Added `DefaultJwtAuthSettings()` class, to unify settings across the services\n7. Added automatic fixture loading for test cases.\n\n\n### -- Version 0.2.3\n1. msb_testing refactored \n2. added new package `msb_const`\n3. Optimized imports throughout\n4. Refactored `msb_devtools`, removed `msb_ext.devtools`\n5. `msb_devtools._exceptions` file removed\n6. Added constant to `mab_auth._constants`\n\n### -- Version 0.2.4\n1. Refactor : (Optimized Imports,Sonarlint warnings)\n2. Refactor : Moved msb_apis.wrappers -> msb_http\n\n### -- Version 0.2.5\n1. Refactor : removed `msb_ext`, as it served no purpose\n2. Fixed : token validation failing due to AUD & ISS claim\n3. Added default fixture paths to `msb_const.paths`\n\n### -- Version 0.2.6\n1. renamed the property `db_query` to `rows`, to make it easier to understand.\n2. added a mentod to deteremine if the current environment is either dev or test env\n3. CrudActions.all is now the default parameter value for `.as_view()` method.\n4. Crud routes not working for single fields\n5. Fixed `self.seriallizer` not working with `dict()`\n6. Implemented `list` Api, to return predefined db columns \n7. search parameter added in crud, searchparameters class refatored\n\n### -- Version 0.2.7\n1. Fixed : `_list_field_names` not working with properties & relations \n2. Added `search_validation_rules` in DefaultRules\n\n### -- Version 0.2.8\n1. Fixed : list api breaking for foreign keys\n2. Fixed : Search parameter not working with fields\n3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.\n\n### -- Version 0.2.9\n1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve \n   that.',
     'author': 'Prakash Mishra',
     'author_email': 'prakash.mishra@intimetec.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `hrin_msb-0.2.8/PKG-INFO` & `hrin_msb-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrin-msb
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Author: Prakash Mishra
 Author-email: prakash.mishra@intimetec.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -175,7 +175,11 @@
 1. Fixed : `_list_field_names` not working with properties & relations 
 2. Added `search_validation_rules` in DefaultRules
 
 ### -- Version 0.2.8
 1. Fixed : list api breaking for foreign keys
 2. Fixed : Search parameter not working with fields
 3. Fixed: automatic encryption of db provate fields, now you need to put `DB_ENCRYPT_PRIVATE_FIELDS = True` to achieve that.
+
+### -- Version 0.2.9
+1. Fixed: automatic encryption of db primary key fields, now you need to put `DB_PK_IS_PRIVATE_FIELD = True` to achieve 
+   that.
```

