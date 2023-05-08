# Comparing `tmp/python_framework-0.4.8.tar.gz` & `tmp/python_framework-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_framework-0.4.8.tar", last modified: Sun Oct 16 01:49:21 2022, max compression
+gzip compressed data, was "python_framework-0.4.9.tar", last modified: Sun Oct 16 02:00:38 2022, max compression
```

## Comparing `python_framework-0.4.8.tar` & `python_framework-0.4.9.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.228089 python_framework-0.4.8/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.454833 python_framework-0.4.8/.github/
--rw-rw-rw-   0        0        0      723 2020-12-10 01:26:12.000000 python_framework-0.4.8/.github/FUNDING.yml
--rw-rw-rw-   0        0        0     1970 2022-09-24 17:39:12.000000 python_framework-0.4.8/.gitignore
--rw-rw-rw-   0        0        0     1090 2020-11-13 13:10:58.000000 python_framework-0.4.8/LICENSE
--rw-rw-rw-   0        0        0      672 2022-10-16 01:49:21.228089 python_framework-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     7581 2022-09-24 05:10:11.000000 python_framework-0.4.8/README.md
--rw-rw-rw-   0        0        0     4088 2022-09-28 01:13:46.000000 python_framework-0.4.8/Tests.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.353105 python_framework-0.4.8/api/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.500711 python_framework-0.4.8/api/resource/
--rw-rw-rw-   0        0        0       21 2021-02-02 10:31:36.000000 python_framework-0.4.8/api/resource/application-local.yml
--rw-rw-rw-   0        0        0      346 2022-09-10 03:33:54.000000 python_framework-0.4.8/api/resource/application.yml
--rw-rw-rw-   0        0        0      558 2022-09-24 05:08:40.000000 python_framework-0.4.8/api/resource/notes.yml
--rw-rw-rw-   0        0        0     8374 2021-10-23 05:56:59.000000 python_framework-0.4.8/api/resource/setting-up-raspberrypi.yml
--rw-rw-rw-   0        0        0     2748 2021-11-15 14:51:03.000000 python_framework-0.4.8/pock.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.512679 python_framework-0.4.8/python_framework/
--rw-rw-rw-   0        0        0     4116 2022-10-13 18:07:11.000000 python_framework-0.4.8/python_framework/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.366070 python_framework-0.4.8/python_framework/api/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.558555 python_framework-0.4.8/python_framework/api/resource/
--rw-rw-rw-   0        0        0        0 2021-05-25 01:46:42.000000 python_framework-0.4.8/python_framework/api/resource/__init__.py
--rw-rw-rw-   0        0        0    26384 2021-10-31 15:41:49.000000 python_framework-0.4.8/python_framework/api/resource/example.json
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.366070 python_framework-0.4.8/python_framework/api/src/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.752038 python_framework-0.4.8/python_framework/api/src/annotation/
--rw-rw-rw-   0        0        0     1840 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/ConverterAnnotation.py
--rw-rw-rw-   0        0        0    11138 2022-06-11 21:57:31.000000 python_framework-0.4.8/python_framework/api/src/annotation/EnumAnnotation.py
--rw-rw-rw-   0        0        0     2118 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/annotation/GlobalExceptionAnnotation.py
--rw-rw-rw-   0        0        0     1826 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/HelperAnnotation.py
--rw-rw-rw-   0        0        0     2011 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/MapperAnnotation.py
--rw-rw-rw-   0        0        0      930 2021-11-07 06:03:07.000000 python_framework-0.4.8/python_framework/api/src/annotation/RepositoryAnnotation.py
--rw-rw-rw-   0        0        0     6981 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/SchedulerAnnotation.py
--rw-rw-rw-   0        0        0     2134 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/ServiceAnnotation.py
--rw-rw-rw-   0        0        0     1876 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/ValidatorAnnotation.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.813872 python_framework-0.4.8/python_framework/api/src/annotation/client/
--rw-rw-rw-   0        0        0     4990 2022-06-11 14:35:43.000000 python_framework-0.4.8/python_framework/api/src/annotation/client/ClientAnnotation.py
--rw-rw-rw-   0        0        0     6339 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/client/EmitterAnnotation.py
--rw-rw-rw-   0        0        0    17717 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/annotation/client/HttpClientAnnotation.py
--rw-rw-rw-   0        0        0     7398 2022-10-13 17:50:24.000000 python_framework-0.4.8/python_framework/api/src/annotation/client/ListenerAnnotation.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.039270 python_framework-0.4.8/python_framework/api/src/constant/
--rw-rw-rw-   0        0        0       25 2022-05-21 00:43:40.000000 python_framework-0.4.8/python_framework/api/src/constant/AuditoryConstant.py
--rw-rw-rw-   0        0        0     1317 2022-04-17 04:39:31.000000 python_framework-0.4.8/python_framework/api/src/constant/ConfigurationKeyConstant.py
--rw-rw-rw-   0        0        0      126 2022-03-05 02:03:19.000000 python_framework-0.4.8/python_framework/api/src/constant/ControllerConstant.py
--rw-rw-rw-   0        0        0       94 2021-11-07 06:30:05.000000 python_framework-0.4.8/python_framework/api/src/constant/HealthCheckConstant.py
--rw-rw-rw-   0        0        0      146 2022-03-25 23:34:32.000000 python_framework-0.4.8/python_framework/api/src/constant/HttpClientConstant.py
--rw-rw-rw-   0        0        0     1078 2022-06-11 14:46:30.000000 python_framework-0.4.8/python_framework/api/src/constant/JwtConstant.py
--rw-rw-rw-   0        0        0      673 2022-03-27 06:49:36.000000 python_framework-0.4.8/python_framework/api/src/constant/LogConstant.py
--rw-rw-rw-   0        0        0      132 2022-09-21 01:24:49.000000 python_framework-0.4.8/python_framework/api/src/constant/SchedulerConstant.py
--rw-rw-rw-   0        0        0       54 2022-03-05 02:36:25.000000 python_framework-0.4.8/python_framework/api/src/constant/StaticConstant.py
--rw-rw-rw-   0        0        0      791 2022-02-22 02:00:55.000000 python_framework-0.4.8/python_framework/api/src/constant/WeekDayConstant.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.078165 python_framework-0.4.8/python_framework/api/src/controller/
--rw-rw-rw-   0        0        0      782 2022-03-04 23:53:15.000000 python_framework-0.4.8/python_framework/api/src/controller/ActuatorHealthController.py
--rw-rw-rw-   0        0        0      718 2022-03-05 01:53:56.000000 python_framework-0.4.8/python_framework/api/src/controller/DocumentationController.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.094122 python_framework-0.4.8/python_framework/api/src/converter/
--rw-rw-rw-   0        0        0      487 2021-04-30 21:48:08.000000 python_framework-0.4.8/python_framework/api/src/converter/ActuatorHealthConverter.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.117061 python_framework-0.4.8/python_framework/api/src/converter/static/
--rw-rw-rw-   0        0        0      567 2022-06-11 14:42:00.000000 python_framework-0.4.8/python_framework/api/src/converter/static/ConverterStatic.py
--rw-rw-rw-   0        0        0     1025 2022-06-11 14:33:42.000000 python_framework-0.4.8/python_framework/api/src/converter/static/StaticConverter.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.126037 python_framework-0.4.8/python_framework/api/src/domain/
--rw-rw-rw-   0        0        0      864 2022-05-11 02:22:11.000000 python_framework-0.4.8/python_framework/api/src/domain/HttpDomain.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.135013 python_framework-0.4.8/python_framework/api/src/dto/
--rw-rw-rw-   0        0        0       98 2021-02-02 10:31:36.000000 python_framework-0.4.8/python_framework/api/src/dto/ActuatorHealthDto.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.181888 python_framework-0.4.8/python_framework/api/src/enumeration/
--rw-rw-rw-   0        0        0      271 2021-02-02 10:31:36.000000 python_framework-0.4.8/python_framework/api/src/enumeration/ActuatorHealthStatus.py
--rw-rw-rw-   0        0        0     3287 2021-04-15 03:36:14.000000 python_framework-0.4.8/python_framework/api/src/enumeration/HttpStatus.py
--rw-rw-rw-   0        0        0      264 2021-04-30 22:38:50.000000 python_framework-0.4.8/python_framework/api/src/enumeration/SchedulerType.py
--rw-rw-rw-   0        0        0      511 2022-02-22 01:57:28.000000 python_framework-0.4.8/python_framework/api/src/enumeration/WeekDay.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.216794 python_framework-0.4.8/python_framework/api/src/model/
--rw-rw-rw-   0        0        0     1457 2022-09-28 15:28:02.000000 python_framework-0.4.8/python_framework/api/src/model/ActuatorHealth.py
--rw-rw-rw-   0        0        0     3470 2022-06-11 14:37:22.000000 python_framework-0.4.8/python_framework/api/src/model/ErrorLog.py
--rw-rw-rw-   0        0        0      279 2021-03-15 01:52:06.000000 python_framework-0.4.8/python_framework/api/src/model/FrameworkModel.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.239733 python_framework-0.4.8/python_framework/api/src/repository/
--rw-rw-rw-   0        0        0      398 2021-04-30 21:49:30.000000 python_framework-0.4.8/python_framework/api/src/repository/ActuatorHealthRepository.py
--rw-rw-rw-   0        0        0      461 2021-10-26 03:55:13.000000 python_framework-0.4.8/python_framework/api/src/repository/DocumentationRepository.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.411275 python_framework-0.4.8/python_framework/api/src/service/
--rw-rw-rw-   0        0        0     1477 2021-11-07 19:32:36.000000 python_framework-0.4.8/python_framework/api/src/service/ActuatorHealthService.py
--rw-rw-rw-   0        0        0    19813 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/service/ApiKeyManager.py
--rw-rw-rw-   0        0        0      528 2022-10-13 18:06:04.000000 python_framework-0.4.8/python_framework/api/src/service/DefaultExceptionManager.py
--rw-rw-rw-   0        0        0      435 2021-10-23 16:16:07.000000 python_framework-0.4.8/python_framework/api/src/service/DocumentationService.py
--rw-rw-rw-   0        0        0    10470 2022-10-13 18:23:00.000000 python_framework-0.4.8/python_framework/api/src/service/ExceptionHandler.py
--rw-rw-rw-   0        0        0     2273 2022-06-12 03:55:18.000000 python_framework-0.4.8/python_framework/api/src/service/SchedulerManager.py
--rw-rw-rw-   0        0        0    20064 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/service/SecurityManager.py
--rw-rw-rw-   0        0        0    19800 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/service/SessionManager.py
--rw-rw-rw-   0        0        0    25559 2022-10-11 21:33:11.000000 python_framework-0.4.8/python_framework/api/src/service/SqlAlchemyProxy.py
--rw-rw-rw-   0        0        0     1787 2022-05-16 16:33:42.000000 python_framework-0.4.8/python_framework/api/src/service/WebBrowser.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.448175 python_framework-0.4.8/python_framework/api/src/service/flask/
--rw-rw-rw-   0        0        0    44185 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/src/service/flask/FlaskManager.py
--rw-rw-rw-   0        0        0    17033 2022-10-13 18:02:17.000000 python_framework-0.4.8/python_framework/api/src/service/flask/ResourceManager.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.501034 python_framework-0.4.8/python_framework/api/src/service/openapi/
--rw-rw-rw-   0        0        0     2288 2021-05-24 21:55:26.000000 python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiDocumentationFile.py
--rw-rw-rw-   0        0        0     1093 2021-10-31 15:52:37.000000 python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiKey.py
--rw-rw-rw-   0        0        0    24486 2022-06-11 14:38:10.000000 python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiManager.py
--rw-rw-rw-   0        0        0      322 2021-11-24 06:36:37.000000 python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiValue.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.553893 python_framework-0.4.8/python_framework/api/src/util/
--rw-rw-rw-   0        0        0     3251 2022-06-11 14:38:33.000000 python_framework-0.4.8/python_framework/api/src/util/AuditoryUtil.py
--rw-rw-rw-   0        0        0    10769 2022-10-16 00:50:40.000000 python_framework-0.4.8/python_framework/api/src/util/ClientUtil.py
--rw-rw-rw-   0        0        0    11104 2022-06-12 00:40:18.000000 python_framework-0.4.8/python_framework/api/src/util/FlaskUtil.py
--rw-rw-rw-   0        0        0    19809 2022-09-30 04:23:48.000000 python_framework-0.4.8/python_framework/api/src/util/Serializer.py
--rw-rw-rw-   0        0        0      430 2021-11-06 17:57:04.000000 python_framework-0.4.8/python_framework/api/src/util/UtcDateTimeUtil.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.571844 python_framework-0.4.8/python_framework/api/test/
--rw-rw-rw-   0        0        0    55283 2022-09-24 07:34:17.000000 python_framework-0.4.8/python_framework/api/test/TestApiTest.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.368066 python_framework-0.4.8/python_framework/api/test/api/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.592788 python_framework-0.4.8/python_framework/api/test/api/resource/
--rw-rw-rw-   0        0        0       21 2021-03-17 21:43:46.000000 python_framework-0.4.8/python_framework/api/test/api/resource/application-local.yml
--rw-rw-rw-   0        0        0       21 2021-03-17 21:43:46.000000 python_framework-0.4.8/python_framework/api/test/api/resource/application-prd.yml
--rw-rw-rw-   0        0        0      404 2021-03-17 21:50:42.000000 python_framework-0.4.8/python_framework/api/test/api/resource/application.yml
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.371057 python_framework-0.4.8/python_framework/api/test/api/src/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.620713 python_framework-0.4.8/python_framework/api/test/api/src/annotation/
--rw-rw-rw-   0        0        0    27895 2021-10-13 07:11:28.000000 python_framework-0.4.8/python_framework/api/test/api/src/annotation/EnumAnnotationTest.py
--rw-rw-rw-   0        0        0     8249 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/test/api/src/annotation/GlobalExceptionAnnotationTest.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.824169 python_framework-0.4.8/python_framework/api/test/api/src/dto/
--rw-rw-rw-   0        0        0       83 2022-04-03 08:46:59.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/MyAttributeClassy.py
--rw-rw-rw-   0        0        0       94 2022-04-03 08:49:35.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/MyAttributeClassyDto.py
--rw-rw-rw-   0        0        0      833 2021-03-17 21:16:48.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/MyDto.py
--rw-rw-rw-   0        0        0      691 2021-03-17 21:16:48.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/MyOtherDto.py
--rw-rw-rw-   0        0        0      733 2021-03-17 21:16:48.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/MyThirdDto.py
--rw-rw-rw-   0        0        0      422 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOf.py
--rw-rw-rw-   0        0        0      412 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfChild.py
--rw-rw-rw-   0        0        0     1268 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfChildDto.py
--rw-rw-rw-   0        0        0      417 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfChildModel.py
--rw-rw-rw-   0        0        0      390 2022-04-03 01:47:24.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfCollection.py
--rw-rw-rw-   0        0        0     1202 2022-04-03 01:47:24.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfCollectionDto.py
--rw-rw-rw-   0        0        0      395 2022-04-03 01:47:24.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfCollectionModel.py
--rw-rw-rw-   0        0        0     1298 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfDto.py
--rw-rw-rw-   0        0        0      427 2022-04-03 02:05:17.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfModel.py
--rw-rw-rw-   0        0        0     1563 2021-03-17 21:17:04.000000 python_framework-0.4.8/python_framework/api/test/api/src/dto/TestCallDto.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.854090 python_framework-0.4.8/python_framework/api/test/api/src/enumeration/
--rw-rw-rw-   0        0        0      305 2021-03-18 04:11:32.000000 python_framework-0.4.8/python_framework/api/test/api/src/enumeration/CallServiceName.py
--rw-rw-rw-   0        0        0      214 2021-03-18 04:11:40.000000 python_framework-0.4.8/python_framework/api/test/api/src/enumeration/CallStatus.py
--rw-rw-rw-   0        0        0      204 2021-03-18 04:11:38.000000 python_framework-0.4.8/python_framework/api/test/api/src/enumeration/CallType.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.899966 python_framework-0.4.8/python_framework/api/test/api/src/service/
--rw-rw-rw-   0        0        0     3377 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/test/api/src/service/ApiKeyManagerTest.py
--rw-rw-rw-   0        0        0     3428 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/test/api/src/service/SecurityManagerTest.py
--rw-rw-rw-   0        0        0     4107 2022-10-13 18:01:53.000000 python_framework-0.4.8/python_framework/api/test/api/src/service/SessionManagerTest.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.912932 python_framework-0.4.8/python_framework/api/test/api/src/service/flask/
--rw-rw-rw-   0        0        0     1020 2022-03-26 00:07:11.000000 python_framework-0.4.8/python_framework/api/test/api/src/service/flask/FlaskManagerTest.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.928890 python_framework-0.4.8/python_framework/api/test/api/src/util/
--rw-rw-rw-   0        0        0    59583 2022-09-10 00:56:16.000000 python_framework-0.4.8/python_framework/api/test/api/src/util/SerializerTest.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.373052 python_framework-0.4.8/python_framework/api/test/apitests/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:20.936869 python_framework-0.4.8/python_framework/api/test/apitests/testone/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.374049 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.020644 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/
--rw-rw-rw-   0        0        0      268 2021-11-06 18:52:42.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-api-key-manager.yml
--rw-rw-rw-   0        0        0      268 2021-11-14 20:18:27.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-client.yml
--rw-rw-rw-   0        0        0      425 2021-11-08 03:32:05.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-dev.yml
--rw-rw-rw-   0        0        0      431 2021-11-08 03:32:05.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-local.yml
--rw-rw-rw-   0        0        0      962 2022-09-24 06:22:48.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-prd.yml
--rw-rw-rw-   0        0        0      229 2021-10-29 03:02:41.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-python-build.yml
--rw-rw-rw-   0        0        0      271 2021-11-02 19:33:30.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-security-manager.yml
--rw-rw-rw-   0        0        0      269 2021-11-03 04:28:43.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-session-manager.yml
--rw-rw-rw-   0        0        0     1213 2022-09-24 05:32:27.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application.yml
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.028622 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/
--rw-rw-rw-   0        0        0      176 2022-09-24 06:32:59.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/TestApi.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.063529 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/
--rw-rw-rw-   0        0        0     4293 2021-11-16 22:17:37.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/ExceptionTestClient.py
--rw-rw-rw-   0        0        0     1843 2021-11-17 02:20:40.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/SomeClient.py
--rw-rw-rw-   0        0        0     4274 2021-11-16 22:17:37.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/TestClient.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.150297 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/
--rw-rw-rw-   0        0        0     4387 2022-09-28 01:15:38.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ActuatorHealthTestController.py
--rw-rw-rw-   0        0        0     3341 2021-11-17 00:45:37.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ApiKeyManagerTestController.py
--rw-rw-rw-   0        0        0     7553 2021-11-15 02:14:21.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ClientExceptionTestController.py
--rw-rw-rw-   0        0        0     9057 2021-11-15 02:13:40.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ClientTestController.py
--rw-rw-rw-   0        0        0     1957 2021-05-23 00:56:50.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/MyController.py
--rw-rw-rw-   0        0        0     3295 2021-11-17 00:45:37.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/SecurityManagerTestController.py
--rw-rw-rw-   0        0        0     3368 2021-11-17 00:45:37.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/SessionManagerTestController.py
--rw-rw-rw-   0        0        0      825 2021-05-23 00:56:24.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/TestCallController.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.161268 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/converter/
--rw-rw-rw-   0        0        0      519 2021-04-30 21:49:02.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/converter/ActuatorHealthTestConverter.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.196174 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/
--rw-rw-rw-   0        0        0      661 2021-11-14 19:16:12.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/ClientTestDto.py
--rw-rw-rw-   0        0        0      235 2021-04-18 04:40:02.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/EnumAsQueryDto.py
--rw-rw-rw-   0        0        0     1563 2021-03-17 21:39:10.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/TestCallDto.py
--rw-rw-rw-   0        0        0      728 2021-11-14 19:15:42.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/TestRequestDto.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.206148 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/model/
--rw-rw-rw-   0        0        0       96 2021-03-18 04:07:24.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/model/ModelAssociation.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.215123 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/repository/
--rw-rw-rw-   0        0        0      391 2022-09-24 10:26:02.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/repository/ActuatorHealthTestRepository.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:21.226096 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/service/
--rw-rw-rw-   0        0        0      765 2022-09-24 17:40:17.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/service/StatusService.py
--rw-rw-rw-   0        0        0     1022 2021-11-15 03:50:06.000000 python_framework-0.4.8/python_framework/api/test/apitests/testone/app.py
-drwxrwxrwx   0        0        0        0 2022-10-16 01:49:19.541601 python_framework-0.4.8/python_framework.egg-info/
--rw-rw-rw-   0        0        0      672 2022-10-16 01:49:19.000000 python_framework-0.4.8/python_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8025 2022-10-16 01:49:19.000000 python_framework-0.4.8/python_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-16 01:49:19.000000 python_framework-0.4.8/python_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      254 2022-10-16 01:49:19.000000 python_framework-0.4.8/python_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0      627 2022-10-16 01:49:19.000000 python_framework-0.4.8/python_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-10-16 01:49:21.231082 python_framework-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     3485 2022-10-16 00:52:16.000000 python_framework-0.4.8/setup.py
--rw-rw-rw-   0        0        0     1074 2022-10-13 18:01:53.000000 python_framework-0.4.8/usage.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.362034 python_framework-0.4.9/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.079789 python_framework-0.4.9/.github/
+-rw-rw-rw-   0        0        0      723 2020-12-10 01:26:12.000000 python_framework-0.4.9/.github/FUNDING.yml
+-rw-rw-rw-   0        0        0     1970 2022-09-24 17:39:12.000000 python_framework-0.4.9/.gitignore
+-rw-rw-rw-   0        0        0     1090 2020-11-13 13:10:58.000000 python_framework-0.4.9/LICENSE
+-rw-rw-rw-   0        0        0      672 2022-10-16 02:00:38.362034 python_framework-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7581 2022-09-24 05:10:11.000000 python_framework-0.4.9/README.md
+-rw-rw-rw-   0        0        0     4088 2022-09-28 01:13:46.000000 python_framework-0.4.9/Tests.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.033912 python_framework-0.4.9/api/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.085774 python_framework-0.4.9/api/resource/
+-rw-rw-rw-   0        0        0       21 2021-02-02 10:31:36.000000 python_framework-0.4.9/api/resource/application-local.yml
+-rw-rw-rw-   0        0        0      346 2022-09-10 03:33:54.000000 python_framework-0.4.9/api/resource/application.yml
+-rw-rw-rw-   0        0        0      558 2022-09-24 05:08:40.000000 python_framework-0.4.9/api/resource/notes.yml
+-rw-rw-rw-   0        0        0     8374 2021-10-23 05:56:59.000000 python_framework-0.4.9/api/resource/setting-up-raspberrypi.yml
+-rw-rw-rw-   0        0        0     2748 2021-11-15 14:51:03.000000 python_framework-0.4.9/pock.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.087769 python_framework-0.4.9/python_framework/
+-rw-rw-rw-   0        0        0     4116 2022-10-13 18:07:11.000000 python_framework-0.4.9/python_framework/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.047875 python_framework-0.4.9/python_framework/api/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.108713 python_framework-0.4.9/python_framework/api/resource/
+-rw-rw-rw-   0        0        0        0 2021-05-25 01:46:42.000000 python_framework-0.4.9/python_framework/api/resource/__init__.py
+-rw-rw-rw-   0        0        0    26384 2021-10-31 15:41:49.000000 python_framework-0.4.9/python_framework/api/resource/example.json
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.046877 python_framework-0.4.9/python_framework/api/src/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.127661 python_framework-0.4.9/python_framework/api/src/annotation/
+-rw-rw-rw-   0        0        0     1840 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/ConverterAnnotation.py
+-rw-rw-rw-   0        0        0    11138 2022-06-11 21:57:31.000000 python_framework-0.4.9/python_framework/api/src/annotation/EnumAnnotation.py
+-rw-rw-rw-   0        0        0     2118 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/annotation/GlobalExceptionAnnotation.py
+-rw-rw-rw-   0        0        0     1826 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/HelperAnnotation.py
+-rw-rw-rw-   0        0        0     2011 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/MapperAnnotation.py
+-rw-rw-rw-   0        0        0      930 2021-11-07 06:03:07.000000 python_framework-0.4.9/python_framework/api/src/annotation/RepositoryAnnotation.py
+-rw-rw-rw-   0        0        0     6981 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/SchedulerAnnotation.py
+-rw-rw-rw-   0        0        0     2134 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/ServiceAnnotation.py
+-rw-rw-rw-   0        0        0     1876 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/ValidatorAnnotation.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.134642 python_framework-0.4.9/python_framework/api/src/annotation/client/
+-rw-rw-rw-   0        0        0     4990 2022-06-11 14:35:43.000000 python_framework-0.4.9/python_framework/api/src/annotation/client/ClientAnnotation.py
+-rw-rw-rw-   0        0        0     6339 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/client/EmitterAnnotation.py
+-rw-rw-rw-   0        0        0    17717 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/annotation/client/HttpClientAnnotation.py
+-rw-rw-rw-   0        0        0     7398 2022-10-13 17:50:24.000000 python_framework-0.4.9/python_framework/api/src/annotation/client/ListenerAnnotation.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.152594 python_framework-0.4.9/python_framework/api/src/constant/
+-rw-rw-rw-   0        0        0       25 2022-05-21 00:43:40.000000 python_framework-0.4.9/python_framework/api/src/constant/AuditoryConstant.py
+-rw-rw-rw-   0        0        0     1317 2022-04-17 04:39:31.000000 python_framework-0.4.9/python_framework/api/src/constant/ConfigurationKeyConstant.py
+-rw-rw-rw-   0        0        0      126 2022-03-05 02:03:19.000000 python_framework-0.4.9/python_framework/api/src/constant/ControllerConstant.py
+-rw-rw-rw-   0        0        0       94 2021-11-07 06:30:05.000000 python_framework-0.4.9/python_framework/api/src/constant/HealthCheckConstant.py
+-rw-rw-rw-   0        0        0      146 2022-03-25 23:34:32.000000 python_framework-0.4.9/python_framework/api/src/constant/HttpClientConstant.py
+-rw-rw-rw-   0        0        0     1078 2022-06-11 14:46:30.000000 python_framework-0.4.9/python_framework/api/src/constant/JwtConstant.py
+-rw-rw-rw-   0        0        0      673 2022-03-27 06:49:36.000000 python_framework-0.4.9/python_framework/api/src/constant/LogConstant.py
+-rw-rw-rw-   0        0        0      132 2022-09-21 01:24:49.000000 python_framework-0.4.9/python_framework/api/src/constant/SchedulerConstant.py
+-rw-rw-rw-   0        0        0       54 2022-03-05 02:36:25.000000 python_framework-0.4.9/python_framework/api/src/constant/StaticConstant.py
+-rw-rw-rw-   0        0        0      791 2022-02-22 02:00:55.000000 python_framework-0.4.9/python_framework/api/src/constant/WeekDayConstant.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.156584 python_framework-0.4.9/python_framework/api/src/controller/
+-rw-rw-rw-   0        0        0      782 2022-03-04 23:53:15.000000 python_framework-0.4.9/python_framework/api/src/controller/ActuatorHealthController.py
+-rw-rw-rw-   0        0        0      718 2022-03-05 01:53:56.000000 python_framework-0.4.9/python_framework/api/src/controller/DocumentationController.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.157581 python_framework-0.4.9/python_framework/api/src/converter/
+-rw-rw-rw-   0        0        0      487 2021-04-30 21:48:08.000000 python_framework-0.4.9/python_framework/api/src/converter/ActuatorHealthConverter.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.161570 python_framework-0.4.9/python_framework/api/src/converter/static/
+-rw-rw-rw-   0        0        0      567 2022-06-11 14:42:00.000000 python_framework-0.4.9/python_framework/api/src/converter/static/ConverterStatic.py
+-rw-rw-rw-   0        0        0     1025 2022-06-11 14:33:42.000000 python_framework-0.4.9/python_framework/api/src/converter/static/StaticConverter.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.163565 python_framework-0.4.9/python_framework/api/src/domain/
+-rw-rw-rw-   0        0        0      864 2022-05-11 02:22:11.000000 python_framework-0.4.9/python_framework/api/src/domain/HttpDomain.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.165560 python_framework-0.4.9/python_framework/api/src/dto/
+-rw-rw-rw-   0        0        0       98 2021-02-02 10:31:36.000000 python_framework-0.4.9/python_framework/api/src/dto/ActuatorHealthDto.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.171543 python_framework-0.4.9/python_framework/api/src/enumeration/
+-rw-rw-rw-   0        0        0      271 2021-02-02 10:31:36.000000 python_framework-0.4.9/python_framework/api/src/enumeration/ActuatorHealthStatus.py
+-rw-rw-rw-   0        0        0     3287 2021-04-15 03:36:14.000000 python_framework-0.4.9/python_framework/api/src/enumeration/HttpStatus.py
+-rw-rw-rw-   0        0        0      264 2021-04-30 22:38:50.000000 python_framework-0.4.9/python_framework/api/src/enumeration/SchedulerType.py
+-rw-rw-rw-   0        0        0      511 2022-02-22 01:57:28.000000 python_framework-0.4.9/python_framework/api/src/enumeration/WeekDay.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.177528 python_framework-0.4.9/python_framework/api/src/model/
+-rw-rw-rw-   0        0        0     1457 2022-09-28 15:28:02.000000 python_framework-0.4.9/python_framework/api/src/model/ActuatorHealth.py
+-rw-rw-rw-   0        0        0     3470 2022-06-11 14:37:22.000000 python_framework-0.4.9/python_framework/api/src/model/ErrorLog.py
+-rw-rw-rw-   0        0        0      279 2021-03-15 01:52:06.000000 python_framework-0.4.9/python_framework/api/src/model/FrameworkModel.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.181517 python_framework-0.4.9/python_framework/api/src/repository/
+-rw-rw-rw-   0        0        0      398 2021-04-30 21:49:30.000000 python_framework-0.4.9/python_framework/api/src/repository/ActuatorHealthRepository.py
+-rw-rw-rw-   0        0        0      461 2021-10-26 03:55:13.000000 python_framework-0.4.9/python_framework/api/src/repository/DocumentationRepository.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.199469 python_framework-0.4.9/python_framework/api/src/service/
+-rw-rw-rw-   0        0        0     1477 2021-11-07 19:32:36.000000 python_framework-0.4.9/python_framework/api/src/service/ActuatorHealthService.py
+-rw-rw-rw-   0        0        0    19813 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/service/ApiKeyManager.py
+-rw-rw-rw-   0        0        0      528 2022-10-13 18:06:04.000000 python_framework-0.4.9/python_framework/api/src/service/DefaultExceptionManager.py
+-rw-rw-rw-   0        0        0      435 2021-10-23 16:16:07.000000 python_framework-0.4.9/python_framework/api/src/service/DocumentationService.py
+-rw-rw-rw-   0        0        0    10470 2022-10-13 18:23:00.000000 python_framework-0.4.9/python_framework/api/src/service/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     2273 2022-06-12 03:55:18.000000 python_framework-0.4.9/python_framework/api/src/service/SchedulerManager.py
+-rw-rw-rw-   0        0        0    20064 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/service/SecurityManager.py
+-rw-rw-rw-   0        0        0    19800 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/service/SessionManager.py
+-rw-rw-rw-   0        0        0    25559 2022-10-11 21:33:11.000000 python_framework-0.4.9/python_framework/api/src/service/SqlAlchemyProxy.py
+-rw-rw-rw-   0        0        0     1787 2022-05-16 16:33:42.000000 python_framework-0.4.9/python_framework/api/src/service/WebBrowser.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.203459 python_framework-0.4.9/python_framework/api/src/service/flask/
+-rw-rw-rw-   0        0        0    44185 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/src/service/flask/FlaskManager.py
+-rw-rw-rw-   0        0        0    17033 2022-10-13 18:02:17.000000 python_framework-0.4.9/python_framework/api/src/service/flask/ResourceManager.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.222410 python_framework-0.4.9/python_framework/api/src/service/openapi/
+-rw-rw-rw-   0        0        0     2288 2021-05-24 21:55:26.000000 python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiDocumentationFile.py
+-rw-rw-rw-   0        0        0     1093 2021-10-31 15:52:37.000000 python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiKey.py
+-rw-rw-rw-   0        0        0    24486 2022-06-11 14:38:10.000000 python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiManager.py
+-rw-rw-rw-   0        0        0      322 2021-11-24 06:36:37.000000 python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiValue.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.231387 python_framework-0.4.9/python_framework/api/src/util/
+-rw-rw-rw-   0        0        0     3251 2022-06-11 14:38:33.000000 python_framework-0.4.9/python_framework/api/src/util/AuditoryUtil.py
+-rw-rw-rw-   0        0        0    10770 2022-10-16 01:59:35.000000 python_framework-0.4.9/python_framework/api/src/util/ClientUtil.py
+-rw-rw-rw-   0        0        0    11104 2022-06-12 00:40:18.000000 python_framework-0.4.9/python_framework/api/src/util/FlaskUtil.py
+-rw-rw-rw-   0        0        0    19809 2022-09-30 04:23:48.000000 python_framework-0.4.9/python_framework/api/src/util/Serializer.py
+-rw-rw-rw-   0        0        0      430 2021-11-06 17:57:04.000000 python_framework-0.4.9/python_framework/api/src/util/UtcDateTimeUtil.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.233378 python_framework-0.4.9/python_framework/api/test/
+-rw-rw-rw-   0        0        0    55283 2022-09-24 07:34:17.000000 python_framework-0.4.9/python_framework/api/test/TestApiTest.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.049870 python_framework-0.4.9/python_framework/api/test/api/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.239362 python_framework-0.4.9/python_framework/api/test/api/resource/
+-rw-rw-rw-   0        0        0       21 2021-03-17 21:43:46.000000 python_framework-0.4.9/python_framework/api/test/api/resource/application-local.yml
+-rw-rw-rw-   0        0        0       21 2021-03-17 21:43:46.000000 python_framework-0.4.9/python_framework/api/test/api/resource/application-prd.yml
+-rw-rw-rw-   0        0        0      404 2021-03-17 21:50:42.000000 python_framework-0.4.9/python_framework/api/test/api/resource/application.yml
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.055856 python_framework-0.4.9/python_framework/api/test/api/src/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.242354 python_framework-0.4.9/python_framework/api/test/api/src/annotation/
+-rw-rw-rw-   0        0        0    27895 2021-10-13 07:11:28.000000 python_framework-0.4.9/python_framework/api/test/api/src/annotation/EnumAnnotationTest.py
+-rw-rw-rw-   0        0        0     8249 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/test/api/src/annotation/GlobalExceptionAnnotationTest.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.273271 python_framework-0.4.9/python_framework/api/test/api/src/dto/
+-rw-rw-rw-   0        0        0       83 2022-04-03 08:46:59.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/MyAttributeClassy.py
+-rw-rw-rw-   0        0        0       94 2022-04-03 08:49:35.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/MyAttributeClassyDto.py
+-rw-rw-rw-   0        0        0      833 2021-03-17 21:16:48.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/MyDto.py
+-rw-rw-rw-   0        0        0      691 2021-03-17 21:16:48.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/MyOtherDto.py
+-rw-rw-rw-   0        0        0      733 2021-03-17 21:16:48.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/MyThirdDto.py
+-rw-rw-rw-   0        0        0      422 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOf.py
+-rw-rw-rw-   0        0        0      412 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfChild.py
+-rw-rw-rw-   0        0        0     1268 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfChildDto.py
+-rw-rw-rw-   0        0        0      417 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfChildModel.py
+-rw-rw-rw-   0        0        0      390 2022-04-03 01:47:24.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfCollection.py
+-rw-rw-rw-   0        0        0     1202 2022-04-03 01:47:24.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfCollectionDto.py
+-rw-rw-rw-   0        0        0      395 2022-04-03 01:47:24.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfCollectionModel.py
+-rw-rw-rw-   0        0        0     1298 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfDto.py
+-rw-rw-rw-   0        0        0      427 2022-04-03 02:05:17.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfModel.py
+-rw-rw-rw-   0        0        0     1563 2021-03-17 21:17:04.000000 python_framework-0.4.9/python_framework/api/test/api/src/dto/TestCallDto.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.289229 python_framework-0.4.9/python_framework/api/test/api/src/enumeration/
+-rw-rw-rw-   0        0        0      305 2021-03-18 04:11:32.000000 python_framework-0.4.9/python_framework/api/test/api/src/enumeration/CallServiceName.py
+-rw-rw-rw-   0        0        0      214 2021-03-18 04:11:40.000000 python_framework-0.4.9/python_framework/api/test/api/src/enumeration/CallStatus.py
+-rw-rw-rw-   0        0        0      204 2021-03-18 04:11:38.000000 python_framework-0.4.9/python_framework/api/test/api/src/enumeration/CallType.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.301196 python_framework-0.4.9/python_framework/api/test/api/src/service/
+-rw-rw-rw-   0        0        0     3377 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/test/api/src/service/ApiKeyManagerTest.py
+-rw-rw-rw-   0        0        0     3428 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/test/api/src/service/SecurityManagerTest.py
+-rw-rw-rw-   0        0        0     4107 2022-10-13 18:01:53.000000 python_framework-0.4.9/python_framework/api/test/api/src/service/SessionManagerTest.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.303192 python_framework-0.4.9/python_framework/api/test/api/src/service/flask/
+-rw-rw-rw-   0        0        0     1020 2022-03-26 00:07:11.000000 python_framework-0.4.9/python_framework/api/test/api/src/service/flask/FlaskManagerTest.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.305186 python_framework-0.4.9/python_framework/api/test/api/src/util/
+-rw-rw-rw-   0        0        0    59583 2022-09-10 00:56:16.000000 python_framework-0.4.9/python_framework/api/test/api/src/util/SerializerTest.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.056851 python_framework-0.4.9/python_framework/api/test/apitests/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.307181 python_framework-0.4.9/python_framework/api/test/apitests/testone/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.058845 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.323138 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/
+-rw-rw-rw-   0        0        0      268 2021-11-06 18:52:42.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-api-key-manager.yml
+-rw-rw-rw-   0        0        0      268 2021-11-14 20:18:27.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-client.yml
+-rw-rw-rw-   0        0        0      425 2021-11-08 03:32:05.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-dev.yml
+-rw-rw-rw-   0        0        0      431 2021-11-08 03:32:05.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-local.yml
+-rw-rw-rw-   0        0        0      962 2022-09-24 06:22:48.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-prd.yml
+-rw-rw-rw-   0        0        0      229 2021-10-29 03:02:41.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-python-build.yml
+-rw-rw-rw-   0        0        0      271 2021-11-02 19:33:30.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-security-manager.yml
+-rw-rw-rw-   0        0        0      269 2021-11-03 04:28:43.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-session-manager.yml
+-rw-rw-rw-   0        0        0     1213 2022-09-24 05:32:27.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application.yml
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.325133 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/
+-rw-rw-rw-   0        0        0      176 2022-09-24 06:32:59.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/TestApi.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.331117 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/
+-rw-rw-rw-   0        0        0     4293 2021-11-16 22:17:37.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/ExceptionTestClient.py
+-rw-rw-rw-   0        0        0     1843 2021-11-17 02:20:40.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/SomeClient.py
+-rw-rw-rw-   0        0        0     4274 2021-11-16 22:17:37.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/TestClient.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.346078 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/
+-rw-rw-rw-   0        0        0     4387 2022-09-28 01:15:38.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ActuatorHealthTestController.py
+-rw-rw-rw-   0        0        0     3341 2021-11-17 00:45:37.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ApiKeyManagerTestController.py
+-rw-rw-rw-   0        0        0     7553 2021-11-15 02:14:21.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ClientExceptionTestController.py
+-rw-rw-rw-   0        0        0     9057 2021-11-15 02:13:40.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ClientTestController.py
+-rw-rw-rw-   0        0        0     1957 2021-05-23 00:56:50.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/MyController.py
+-rw-rw-rw-   0        0        0     3295 2021-11-17 00:45:37.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/SecurityManagerTestController.py
+-rw-rw-rw-   0        0        0     3368 2021-11-17 00:45:37.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/SessionManagerTestController.py
+-rw-rw-rw-   0        0        0      825 2021-05-23 00:56:24.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/TestCallController.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.348071 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/converter/
+-rw-rw-rw-   0        0        0      519 2021-04-30 21:49:02.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/converter/ActuatorHealthTestConverter.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.355053 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/
+-rw-rw-rw-   0        0        0      661 2021-11-14 19:16:12.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/ClientTestDto.py
+-rw-rw-rw-   0        0        0      235 2021-04-18 04:40:02.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/EnumAsQueryDto.py
+-rw-rw-rw-   0        0        0     1563 2021-03-17 21:39:10.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/TestCallDto.py
+-rw-rw-rw-   0        0        0      728 2021-11-14 19:15:42.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/TestRequestDto.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.357047 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/model/
+-rw-rw-rw-   0        0        0       96 2021-03-18 04:07:24.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/model/ModelAssociation.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.358044 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/repository/
+-rw-rw-rw-   0        0        0      391 2022-09-24 10:26:02.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/repository/ActuatorHealthTestRepository.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.360039 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/service/
+-rw-rw-rw-   0        0        0      765 2022-09-24 17:40:17.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/service/StatusService.py
+-rw-rw-rw-   0        0        0     1022 2021-11-15 03:50:06.000000 python_framework-0.4.9/python_framework/api/test/apitests/testone/app.py
+drwxrwxrwx   0        0        0        0 2022-10-16 02:00:38.105720 python_framework-0.4.9/python_framework.egg-info/
+-rw-rw-rw-   0        0        0      672 2022-10-16 02:00:37.000000 python_framework-0.4.9/python_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8025 2022-10-16 02:00:37.000000 python_framework-0.4.9/python_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-16 02:00:37.000000 python_framework-0.4.9/python_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      254 2022-10-16 02:00:37.000000 python_framework-0.4.9/python_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      627 2022-10-16 02:00:37.000000 python_framework-0.4.9/python_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-10-16 02:00:38.365026 python_framework-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     3485 2022-10-16 01:59:50.000000 python_framework-0.4.9/setup.py
+-rw-rw-rw-   0        0        0     1074 2022-10-13 18:01:53.000000 python_framework-0.4.9/usage.py
```

### Comparing `python_framework-0.4.8/.github/FUNDING.yml` & `python_framework-0.4.9/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/.gitignore` & `python_framework-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/LICENSE` & `python_framework-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/PKG-INFO` & `python_framework-0.4.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python_framework
-Version: 0.4.8
+Version: 0.4.9
 Summary: Flask wrapper
 Home-page: https://github.com/SamuelJansen/python-framework/
-Download-URL: https://github.com/SamuelJansen/python-framework/archive/v0.4.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/python-framework/archive/v0.4.9.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: flask,sqlalchemy,open api,jwt,serializer,scheduler
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python_framework-0.4.8/README.md` & `python_framework-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/Tests.py` & `python_framework-0.4.9/Tests.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/api/resource/notes.yml` & `python_framework-0.4.9/api/resource/notes.yml`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/api/resource/setting-up-raspberrypi.yml` & `python_framework-0.4.9/api/resource/setting-up-raspberrypi.yml`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/pock.py` & `python_framework-0.4.9/pock.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/__init__.py` & `python_framework-0.4.9/python_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/resource/example.json` & `python_framework-0.4.9/python_framework/api/resource/example.json`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/ConverterAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/ConverterAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/EnumAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/EnumAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/GlobalExceptionAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/GlobalExceptionAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/HelperAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/HelperAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/MapperAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/MapperAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/RepositoryAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/RepositoryAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/SchedulerAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/SchedulerAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/ServiceAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/ServiceAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/ValidatorAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/ValidatorAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/client/ClientAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/client/ClientAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/client/EmitterAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/client/EmitterAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/client/HttpClientAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/client/HttpClientAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/annotation/client/ListenerAnnotation.py` & `python_framework-0.4.9/python_framework/api/src/annotation/client/ListenerAnnotation.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/constant/ConfigurationKeyConstant.py` & `python_framework-0.4.9/python_framework/api/src/constant/ConfigurationKeyConstant.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/constant/JwtConstant.py` & `python_framework-0.4.9/python_framework/api/src/constant/JwtConstant.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/constant/LogConstant.py` & `python_framework-0.4.9/python_framework/api/src/constant/LogConstant.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/constant/WeekDayConstant.py` & `python_framework-0.4.9/python_framework/api/src/constant/WeekDayConstant.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/controller/ActuatorHealthController.py` & `python_framework-0.4.9/python_framework/api/src/controller/ActuatorHealthController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/controller/DocumentationController.py` & `python_framework-0.4.9/python_framework/api/src/controller/DocumentationController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/converter/static/ConverterStatic.py` & `python_framework-0.4.9/python_framework/api/src/converter/static/ConverterStatic.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/converter/static/StaticConverter.py` & `python_framework-0.4.9/python_framework/api/src/converter/static/StaticConverter.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/domain/HttpDomain.py` & `python_framework-0.4.9/python_framework/api/src/domain/HttpDomain.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/enumeration/HttpStatus.py` & `python_framework-0.4.9/python_framework/api/src/enumeration/HttpStatus.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/model/ActuatorHealth.py` & `python_framework-0.4.9/python_framework/api/src/model/ActuatorHealth.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/model/ErrorLog.py` & `python_framework-0.4.9/python_framework/api/src/model/ErrorLog.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/ActuatorHealthService.py` & `python_framework-0.4.9/python_framework/api/src/service/ActuatorHealthService.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/ApiKeyManager.py` & `python_framework-0.4.9/python_framework/api/src/service/ApiKeyManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/DefaultExceptionManager.py` & `python_framework-0.4.9/python_framework/api/src/service/DefaultExceptionManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/ExceptionHandler.py` & `python_framework-0.4.9/python_framework/api/src/service/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/SchedulerManager.py` & `python_framework-0.4.9/python_framework/api/src/service/SchedulerManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/SecurityManager.py` & `python_framework-0.4.9/python_framework/api/src/service/SecurityManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/SessionManager.py` & `python_framework-0.4.9/python_framework/api/src/service/SessionManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/SqlAlchemyProxy.py` & `python_framework-0.4.9/python_framework/api/src/service/SqlAlchemyProxy.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/WebBrowser.py` & `python_framework-0.4.9/python_framework/api/src/service/WebBrowser.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/flask/FlaskManager.py` & `python_framework-0.4.9/python_framework/api/src/service/flask/FlaskManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/flask/ResourceManager.py` & `python_framework-0.4.9/python_framework/api/src/service/flask/ResourceManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiDocumentationFile.py` & `python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiDocumentationFile.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiKey.py` & `python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiKey.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/service/openapi/OpenApiManager.py` & `python_framework-0.4.9/python_framework/api/src/service/openapi/OpenApiManager.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/util/AuditoryUtil.py` & `python_framework-0.4.9/python_framework/api/src/util/AuditoryUtil.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/util/ClientUtil.py` & `python_framework-0.4.9/python_framework/api/src/util/ClientUtil.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     try:
         evenOrCompleteResponse = resourceInstanceMethod(*args, **kwargs)
         if isinstance(evenOrCompleteResponse, HttpClientEvent):
             return evenOrCompleteResponse
         else:
             return ManualHttpClientEvent(evenOrCompleteResponse, *args, **kwargs)
     except Exception as exception:
-        log.log(getHttpClientEvent, 'Not possible o get client event' exception=exception)
+        log.log(getHttpClientEvent, 'Not possible o get client event', exception=exception)
         raise exception
 
 
 def raiseHttpClientEventNotFoundException(*args, **kwargs):
     raise Exception('HttpClientEvent not found')
```

### Comparing `python_framework-0.4.8/python_framework/api/src/util/FlaskUtil.py` & `python_framework-0.4.9/python_framework/api/src/util/FlaskUtil.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/src/util/Serializer.py` & `python_framework-0.4.9/python_framework/api/src/util/Serializer.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/TestApiTest.py` & `python_framework-0.4.9/python_framework/api/test/TestApiTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/annotation/EnumAnnotationTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/annotation/EnumAnnotationTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/annotation/GlobalExceptionAnnotationTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/annotation/GlobalExceptionAnnotationTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/MyDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/MyDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/MyOtherDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/MyOtherDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/MyThirdDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/MyThirdDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfChildDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfChildDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfCollectionDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfCollectionDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/SomeExampleOfDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/SomeExampleOfDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/dto/TestCallDto.py` & `python_framework-0.4.9/python_framework/api/test/api/src/dto/TestCallDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/service/ApiKeyManagerTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/service/ApiKeyManagerTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/service/SecurityManagerTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/service/SecurityManagerTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/service/SessionManagerTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/service/SessionManagerTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/service/flask/FlaskManagerTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/service/flask/FlaskManagerTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/api/src/util/SerializerTest.py` & `python_framework-0.4.9/python_framework/api/test/api/src/util/SerializerTest.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application-prd.yml` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application-prd.yml`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/resource/application.yml` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/resource/application.yml`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/ExceptionTestClient.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/ExceptionTestClient.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/SomeClient.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/SomeClient.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/client/TestClient.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/client/TestClient.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ActuatorHealthTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ActuatorHealthTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ApiKeyManagerTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ApiKeyManagerTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ClientExceptionTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ClientExceptionTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/ClientTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/ClientTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/MyController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/MyController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/SecurityManagerTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/SecurityManagerTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/SessionManagerTestController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/SessionManagerTestController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/controller/TestCallController.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/controller/TestCallController.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/converter/ActuatorHealthTestConverter.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/converter/ActuatorHealthTestConverter.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/ClientTestDto.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/ClientTestDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/TestCallDto.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/TestCallDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/dto/TestRequestDto.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/dto/TestRequestDto.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/api/src/service/StatusService.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/api/src/service/StatusService.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework/api/test/apitests/testone/app.py` & `python_framework-0.4.9/python_framework/api/test/apitests/testone/app.py`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework.egg-info/PKG-INFO` & `python_framework-0.4.9/python_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: python-framework
-Version: 0.4.8
+Version: 0.4.9
 Summary: Flask wrapper
 Home-page: https://github.com/SamuelJansen/python-framework/
-Download-URL: https://github.com/SamuelJansen/python-framework/archive/v0.4.8.tar.gz
+Download-URL: https://github.com/SamuelJansen/python-framework/archive/v0.4.9.tar.gz
 Author: Samuel Jansen
 Author-email: samuel.jansenn@gmail.com
 License: MIT
 Keywords: flask,sqlalchemy,open api,jwt,serializer,scheduler
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `python_framework-0.4.8/python_framework.egg-info/SOURCES.txt` & `python_framework-0.4.9/python_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/python_framework.egg-info/top_level.txt` & `python_framework-0.4.9/python_framework.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `python_framework-0.4.8/setup.py` & `python_framework-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 sudo rm /usr/bin/python
 sudo ln -s /usr/local/bin/pythonX.Y /usr/bin/python
 
 sudo rm /usr/bin/pip
 sudo ln -s /usr/local/bin/pipX.Y /usr/bin/pip
 ''')
 
-VERSION = '0.4.8'
+VERSION = '0.4.9'
 
 NAME = 'python_framework'
 PACKAGE_NAME = NAME
 REPOSITORY_NAME = NAME.replace("_", "-")
 URL = f'https://github.com/SamuelJansen/{REPOSITORY_NAME}/'
 
 OS_SEPARATOR = os.path.sep
```

### Comparing `python_framework-0.4.8/usage.py` & `python_framework-0.4.9/usage.py`

 * *Files identical despite different names*

