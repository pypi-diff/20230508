# Comparing `tmp/heaserver-1.0.0a98.tar.gz` & `tmp/heaserver-1.0.0a99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.0.0a98.tar", last modified: Sat Feb 11 01:38:36 2023, max compression
+gzip compressed data, was "heaserver-1.0.0a99.tar", last modified: Tue Feb 14 17:20:07 2023, max compression
```

## Comparing `heaserver-1.0.0a98.tar` & `heaserver-1.0.0a99.tar`

### file list

```diff
@@ -1,187 +1,189 @@
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.374564 heaserver-1.0.0a98/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/.editorconfig
--rw-rw-rw-   0        0        0      286 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/LICENSE
--rw-rw-rw-   0        0        0      243 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/MANIFEST.in
--rw-rw-rw-   0        0        0     3631 2023-02-11 01:38:36.373566 heaserver-1.0.0a98/PKG-INFO
--rw-rw-rw-   0        0        0     2447 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/README.md
--rw-rw-rw-   0        0        0     1603 2022-08-18 21:02:53.000000 heaserver-1.0.0a98/RELEASING.md
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.221594 heaserver-1.0.0a98/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.221594 heaserver-1.0.0a98/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.238564 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34361 2023-02-10 19:12:28.000000 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0    30101 2023-01-26 23:36:04.000000 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0     1309 2022-08-18 21:02:53.000000 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.239564 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-02-06 04:26:32.000000 heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.222565 heaserver-1.0.0a98/awss3tests/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.222565 heaserver-1.0.0a98/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.243564 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    35055 2023-02-10 19:12:34.000000 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0    30242 2023-01-28 04:03:43.000000 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0     1309 2022-08-18 21:02:53.000000 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.243564 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    17565 2023-02-06 04:26:25.000000 heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.224564 heaserver-1.0.0a98/integrationtests/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.224564 heaserver-1.0.0a98/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.258569 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     6306 2022-11-01 21:34:36.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5417 2022-11-01 21:34:29.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5417 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     4964 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12867 2022-06-17 21:25:43.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1193 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2022-03-30 20:48:21.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2022-05-27 00:02:51.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4619 2023-01-26 23:37:53.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2022-05-27 00:02:51.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.259567 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      115 2022-10-07 23:39:41.000000 heaserver-1.0.0a98/pytest.ini
--rw-rw-rw-   0        0        0      239 2022-11-01 22:14:02.000000 heaserver-1.0.0a98/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2023-02-11 01:38:36.374564 heaserver-1.0.0a98/setup.cfg
--rw-rw-rw-   0        0        0     2647 2023-02-11 01:37:58.000000 heaserver-1.0.0a98/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.225565 heaserver-1.0.0a98/src/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.225565 heaserver-1.0.0a98/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.293564 heaserver-1.0.0a98/src/heaserver/service/
--rw-rw-rw-   0        0        0       79 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0    17005 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1582 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      686 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     1497 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-02-11 01:27:18.000000 heaserver-1.0.0a98/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    11915 2023-01-21 03:18:23.000000 heaserver-1.0.0a98/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2520 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/config.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.301564 heaserver-1.0.0a98/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    17452 2023-02-07 15:41:53.000000 heaserver-1.0.0a98/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0     3883 2023-02-07 19:22:42.000000 heaserver-1.0.0a98/src/heaserver/service/db/awss3bucketobjectkey.py
--rw-rw-rw-   0        0        0   116803 2023-02-10 23:25:45.000000 heaserver-1.0.0a98/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    23369 2023-01-21 03:18:23.000000 heaserver-1.0.0a98/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    20020 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4111 2022-04-18 21:29:43.000000 heaserver-1.0.0a98/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    12772 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      773 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    15440 2023-02-07 19:14:03.000000 heaserver-1.0.0a98/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      557 2023-01-27 17:14:14.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.305565 heaserver-1.0.0a98/src/heaserver/service/jsonschemas/
--rw-rw-rw-   0        0        0      900 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschemas/cjtemplate.json
--rw-rw-rw-   0        0        0      197 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschemas/nvpjson.json
--rw-rw-rw-   0        0        0     2402 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschemas/wstl.json
--rw-rw-rw-   0        0        0     5083 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschemas/wstlaction.json
--rw-rw-rw-   0        0        0      661 2023-01-27 17:07:26.000000 heaserver-1.0.0a98/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    18612 2022-10-31 23:07:25.000000 heaserver-1.0.0a98/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2022-04-20 00:03:32.000000 heaserver-1.0.0a98/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.312564 heaserver-1.0.0a98/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1217 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    23174 2023-01-28 01:11:39.000000 heaserver-1.0.0a98/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     3353 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2107 2022-03-24 03:01:02.000000 heaserver-1.0.0a98/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3091 2022-04-18 21:29:43.000000 heaserver-1.0.0a98/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1410 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1645 2022-07-19 18:00:24.000000 heaserver-1.0.0a98/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    22754 2023-02-11 01:33:04.000000 heaserver-1.0.0a98/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    11928 2022-11-02 20:01:00.000000 heaserver-1.0.0a98/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       60 2022-04-20 00:03:32.000000 heaserver-1.0.0a98/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.324564 heaserver-1.0.0a98/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2022-06-10 16:41:10.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     4322 2023-01-26 23:35:02.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    19142 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6354 2023-01-26 23:49:52.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     6664 2023-01-27 00:53:33.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    38124 2023-01-31 05:30:01.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    14969 2023-01-31 05:04:48.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   133696 2022-11-03 23:22:04.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0     9926 2023-02-04 20:48:23.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0    12742 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      477 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7538 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    28492 2023-01-27 01:04:49.000000 heaserver-1.0.0a98/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2877 2023-01-30 16:44:41.000000 heaserver-1.0.0a98/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0     7027 2023-01-30 16:44:41.000000 heaserver-1.0.0a98/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    22030 2023-01-30 22:16:30.000000 heaserver-1.0.0a98/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.272565 heaserver-1.0.0a98/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     3631 2023-02-11 01:38:36.000000 heaserver-1.0.0a98/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7453 2023-02-11 01:38:36.000000 heaserver-1.0.0a98/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-11 01:38:36.000000 heaserver-1.0.0a98/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      385 2023-02-11 01:38:36.000000 heaserver-1.0.0a98/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-11 01:38:36.000000 heaserver-1.0.0a98/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.227564 heaserver-1.0.0a98/tests/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.227564 heaserver-1.0.0a98/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.356563 heaserver-1.0.0a98/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/__init__.py
--rw-rw-rw-   0        0        0     6355 2022-11-01 21:33:59.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    12731 2022-11-01 21:33:51.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.359563 heaserver-1.0.0a98/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/db/__init__.py
--rw-rw-rw-   0        0        0      551 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7291 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5280 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5548 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.371563 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/__init__.py
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    46477 2023-01-22 17:59:57.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4176 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     4249 2022-03-11 17:59:13.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2560 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13078 2023-01-28 01:07:18.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     2506 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     3076 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      204 2022-05-27 00:02:51.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0      405 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2022-05-27 00:02:51.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5289 2022-11-03 23:22:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0     1005 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2022-06-24 01:06:04.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2022-05-27 00:02:51.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2022-04-18 21:29:43.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2022-10-25 23:19:43.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2022-07-12 22:55:17.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6281 2023-01-30 16:44:41.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2023-02-11 01:38:36.372563 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16440 2022-06-30 18:56:03.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:07.125933 heaserver-1.0.0a99/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/.editorconfig
+-rw-rw-rw-   0        0        0      286 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/LICENSE
+-rw-rw-rw-   0        0        0      243 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/MANIFEST.in
+-rw-rw-rw-   0        0        0     3631 2023-02-14 17:20:07.125933 heaserver-1.0.0a99/PKG-INFO
+-rw-rw-rw-   0        0        0     2447 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/README.md
+-rw-rw-rw-   0        0        0     1603 2022-08-18 21:02:53.000000 heaserver-1.0.0a99/RELEASING.md
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.354748 heaserver-1.0.0a99/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.354748 heaserver-1.0.0a99/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.411187 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34361 2023-02-10 19:12:28.000000 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0    30101 2023-01-26 23:36:04.000000 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0     1309 2022-08-18 21:02:53.000000 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.417188 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-02-06 04:26:32.000000 heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.354748 heaserver-1.0.0a99/awss3tests/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.354748 heaserver-1.0.0a99/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.436616 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    35055 2023-02-10 19:12:34.000000 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0    30242 2023-01-28 04:03:43.000000 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0     1309 2022-08-18 21:02:53.000000 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.441584 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    17565 2023-02-06 04:26:25.000000 heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/integrationtests/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.516681 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     6306 2022-11-01 21:34:36.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5417 2022-11-01 21:34:29.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5417 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     4964 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12867 2022-06-17 21:25:43.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1193 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2022-03-30 20:48:21.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2022-05-27 00:02:51.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4619 2023-01-26 23:37:53.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2022-05-27 00:02:51.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.516681 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      115 2022-10-07 23:39:41.000000 heaserver-1.0.0a99/pytest.ini
+-rw-rw-rw-   0        0        0      239 2022-11-01 22:14:02.000000 heaserver-1.0.0a99/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-02-14 17:20:07.125933 heaserver-1.0.0a99/setup.cfg
+-rw-rw-rw-   0        0        0     2678 2023-02-14 17:19:34.000000 heaserver-1.0.0a99/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/src/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.688572 heaserver-1.0.0a99/src/heaserver/service/
+-rw-rw-rw-   0        0        0       79 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0    17843 2023-02-11 20:10:39.000000 heaserver-1.0.0a99/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1582 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      686 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     1497 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-02-11 01:27:18.000000 heaserver-1.0.0a99/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    11915 2023-01-21 03:18:23.000000 heaserver-1.0.0a99/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2520 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/config.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.735353 heaserver-1.0.0a99/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    17177 2023-02-14 03:51:04.000000 heaserver-1.0.0a99/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0     3883 2023-02-07 19:22:42.000000 heaserver-1.0.0a99/src/heaserver/service/db/awss3bucketobjectkey.py
+-rw-rw-rw-   0        0        0   118081 2023-02-14 04:44:54.000000 heaserver-1.0.0a99/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    23369 2023-01-21 03:18:23.000000 heaserver-1.0.0a99/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    20020 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4111 2022-04-18 21:29:43.000000 heaserver-1.0.0a99/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    12772 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0     4361 2023-02-13 16:04:20.000000 heaserver-1.0.0a99/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    15440 2023-02-07 19:14:03.000000 heaserver-1.0.0a99/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      557 2023-01-27 17:14:14.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.751018 heaserver-1.0.0a99/src/heaserver/service/jsonschemas/
+-rw-rw-rw-   0        0        0      900 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschemas/cjtemplate.json
+-rw-rw-rw-   0        0        0      197 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschemas/nvpjson.json
+-rw-rw-rw-   0        0        0     2402 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschemas/wstl.json
+-rw-rw-rw-   0        0        0     5083 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschemas/wstlaction.json
+-rw-rw-rw-   0        0        0      661 2023-01-27 17:07:26.000000 heaserver-1.0.0a99/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    18612 2022-10-31 23:07:25.000000 heaserver-1.0.0a99/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2022-04-20 00:03:32.000000 heaserver-1.0.0a99/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.797814 heaserver-1.0.0a99/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1217 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    23174 2023-01-28 01:11:39.000000 heaserver-1.0.0a99/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     3353 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2107 2022-03-24 03:01:02.000000 heaserver-1.0.0a99/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3091 2022-04-18 21:29:43.000000 heaserver-1.0.0a99/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1410 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1645 2022-07-19 18:00:24.000000 heaserver-1.0.0a99/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    22754 2023-02-11 01:33:04.000000 heaserver-1.0.0a99/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    11928 2022-11-02 20:01:00.000000 heaserver-1.0.0a99/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       60 2022-04-20 00:03:32.000000 heaserver-1.0.0a99/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.860218 heaserver-1.0.0a99/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2022-06-10 16:41:10.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     4322 2023-01-26 23:35:02.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    19142 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6354 2023-01-26 23:49:52.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     6664 2023-01-27 00:53:33.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40010 2023-02-14 06:18:23.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    14998 2023-02-14 04:04:46.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   133696 2022-11-03 23:22:04.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0     9912 2023-02-14 05:34:54.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0    12742 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      477 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7538 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    28742 2023-02-14 00:03:25.000000 heaserver-1.0.0a99/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2877 2023-01-30 16:44:41.000000 heaserver-1.0.0a99/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0     7027 2023-01-30 16:44:41.000000 heaserver-1.0.0a99/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    22030 2023-01-30 22:16:30.000000 heaserver-1.0.0a99/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.532313 heaserver-1.0.0a99/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     3631 2023-02-14 17:20:06.000000 heaserver-1.0.0a99/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7536 2023-02-14 17:20:06.000000 heaserver-1.0.0a99/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-14 17:20:06.000000 heaserver-1.0.0a99/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      404 2023-02-14 17:20:06.000000 heaserver-1.0.0a99/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-02-14 17:20:06.000000 heaserver-1.0.0a99/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/tests/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:06.360251 heaserver-1.0.0a99/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:07.047892 heaserver-1.0.0a99/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/__init__.py
+-rw-rw-rw-   0        0        0     6355 2022-11-01 21:33:59.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    12731 2022-11-01 21:33:51.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:07.047892 heaserver-1.0.0a99/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/db/__init__.py
+-rw-rw-rw-   0        0        0      551 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7291 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5280 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5548 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:07.110269 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/__init__.py
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    46477 2023-01-22 17:59:57.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4176 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     4249 2022-03-11 17:59:13.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2560 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13078 2023-01-28 01:07:18.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     2506 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     3076 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      204 2022-05-27 00:02:51.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     4282 2023-02-13 16:33:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2022-05-27 00:02:51.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5289 2022-11-03 23:22:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0     1005 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2022-06-24 01:06:04.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2022-05-27 00:02:51.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2022-04-18 21:29:43.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2022-10-25 23:19:43.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2022-07-12 22:55:17.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6281 2023-01-30 16:44:41.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2023-02-14 17:20:07.125933 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16440 2022-06-30 18:56:03.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.0.0a98/LICENSE` & `heaserver-1.0.0a99/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/PKG-INFO` & `heaserver-1.0.0a99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.0.0a98
+Version: 1.0.0a99
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `heaserver-1.0.0a98/README.md` & `heaserver-1.0.0a99/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/RELEASING.md` & `heaserver-1.0.0a99/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.0.0a99/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/service.py` & `heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/awss3tests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.0.0a99/awss3tests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.0.0a99/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/setup.py` & `heaserver-1.0.0a99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.0.0a98',
+      version='1.0.0a99',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
@@ -39,16 +39,16 @@
           'boto3==1.21.38',
           'botocore==1.24.38',
           'boto3-stubs[essential]==1.21.38',
           'botocore-stubs[essential]==1.24.38',
           'freezegun~=1.0.0',  # Need an old version of freezegun for https://github.com/spulec/freezegun/issues/437
           'regex~=2022.4.24',
           'aio-pika==8.1.0',
-          'PyJWT==2.6.0'
-
+          'PyJWT==2.6.0',
+          'simpleeval~=0.9.12'
       ],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/aiohttp.py` & `heaserver-1.0.0a99/src/heaserver/service/aiohttp.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from aiohttp.client import ClientSession
 from typing import Protocol, AsyncIterator, BinaryIO
 from heaobject.root import json_dumps
 from contextlib import asynccontextmanager
 import logging
 import os
 import platform
+import time
 
 if platform.system() == 'Windows':
     try:
         import msvcrt
         from ctypes import windll, byref, wintypes, GetLastError, WinError, POINTER
         from ctypes.wintypes import HANDLE, DWORD, BOOL
         LPDWORD = POINTER(wintypes.DWORD)
@@ -397,21 +398,24 @@
         :param loop: the current event loop. If None, it will use asyncio.get_running_loop().
         """
         if loop is not None:
             self.loop = loop
         else:
             self.loop = asyncio.get_running_loop()
         self.request = request
+        self.__pump_task: asyncio.Task | None = None
+        self.__reader: BinaryIO | None = None
+        self.__writer: BinaryIO | None = None
 
     def initialize(self):
         """
         Creates resources needed for reading.
         """
         read_fd, write_fd = os.pipe()
-        self.loop.create_task(self.__pump_bytes_into_fd())
+        self.__pump_task = self.loop.create_task(self.__pump_bytes_into_fd())
         self.__reader = os.fdopen(read_fd, 'rb')
         self.__writer = os.fdopen(write_fd, 'wb')
 
     def read(self, n=-1) -> bytes:
         """
         Reads some bytes.
 
@@ -427,25 +431,41 @@
     def close(self):
         """
         Cleans up all resources in this file-like object.
         """
         logger = logging.getLogger(__name__)
         logger.debug('Closing')
         try:
-            self.__writer.close()
-            self.__reader.close()
+            if self.__writer is not None:
+                self.__writer.close()
+                self.__writer = None
+            if self.__reader is not None:
+                self.__reader.close()
+                self.__reader = None
+            while self.__pump_task is not None and not self.__pump_task.done():
+                time.sleep(0.1)
+            self.__pump_task = None
         except Exception as e:
             logger.exception('Failed to close pipe')
+            if self.__reader is not None:
+                try:
+                    self.__reader.close()
+                    self.__reader = None
+                except Exception:
+                    pass
             try:
-                self.__reader.close()
+                while self.__pump_task is not None and not self.__pump_task.done():
+                    time.sleep(0.1)
+                self.__pump_task = None
             except Exception:
                 pass
             raise e
 
 
+
     async def __pump_bytes_into_fd(self):
         logger = logging.getLogger(__name__)
         writer_closed = False
         try:
             while not self.request.content.at_eof():
                 logger.debug('About to read chunk')
                 chunk = await self.request.content.read(CHUNK_SIZE)
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/appfactory.py` & `heaserver-1.0.0a99/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/appproperty.py` & `heaserver-1.0.0a99/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/caching.py` & `heaserver-1.0.0a99/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/client.py` & `heaserver-1.0.0a99/src/heaserver/service/client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/config.py` & `heaserver-1.0.0a99/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/aws.py` & `heaserver-1.0.0a99/src/heaserver/service/db/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,23 +267,15 @@
         for bucket_dict in v:
             awsbucket = AWSBucket()
             awsbucket.from_dict(bucket_dict)
             cls.__create_bucket(awsbucket)
 
     @classmethod
     def __awsaccount_inserter(cls, v):
-        for awsaccount_dict in v:
-            awsaccount = AWSAccount()
-            awsaccount.from_dict(awsaccount_dict)
-            cls.__create_awsaccount(awsaccount)
-
-    @staticmethod
-    def __create_awsaccount(account: AWSAccount):
-        client = boto3.client('organizations')
-        client.create_account(Email=account.email_address, AccountName=account.display_name)
+        pass  # moto automatically creates one account to use. Creating your own accounts doesn't seem to work.
 
     @staticmethod
     def __create_bucket(bucket: AWSBucket):
         client = boto3.client('s3')
         if bucket is not None:
             if bucket.name is None:
                 raise ValueError('bucket.name cannot be None')
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/awss3bucketobjectkey.py` & `heaserver-1.0.0a99/src/heaserver/service/db/awss3bucketobjectkey.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.0.0a99/src/heaserver/service/db/awsservicelib.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,42 @@
     account, volume_id = next((a for a in await gather(
         *[get_account_and_volume_id(_get_account(request, v.id), v.id) async for v in
           request.app[HEA_DB].get_volumes(request, AWSFileSystem)])
                                if a[0]['id'] == request.match_info['id']), (None, None))
     return account, volume_id
 
 
+async def get_account_by_name(request: web.Request) -> tuple[DesktopObjectDict | None, str | None]:
+    """
+    Gets an account by its id and the account's volume id. The id is expected to be the request object's match_info
+    mapping, with key 'id'.
+
+    :param request: an aiohttp Request object (required).
+    :return: a two-tuple containing an AWSAccount dict and volume id.
+    """
+
+    async def get_account_and_volume_id(account_getter: Awaitable[DesktopObjectDict | None],
+                                        volume_id_: str | None) -> tuple[DesktopObjectDict | None, str | None]:
+        """
+        This function serves as a pass-through for volume ids so we can return the volume id along with the account
+        dict.
+
+        :param account_getter: the actual coroutine to get the account.
+        :param volume_id_: the volume id.
+        :return: a two-tuple containing the account dict and the volume id.
+        """
+        return await account_getter, volume_id_
+
+    account, volume_id = next((a for a in await gather(
+        *[get_account_and_volume_id(_get_account(request, v.id), v.id) async for v in
+          request.app[HEA_DB].get_volumes(request, AWSFileSystem)])
+                               if a[0]['id'] == request.match_info['name']), (None, None))
+    return account, volume_id
+
+
 async def get_volume_id_for_account_id(request: web.Request) -> Optional[str]:
     """
     Gets the id of the volume associated with an AWS account. The account id is expected to be in the request object's
     match_info mapping, with key 'id'.
 
     :param request: an aiohttp Request object (required).
     :return: a volume id string, or None if no volume was found associated with the AWS account.
@@ -2040,15 +2068,14 @@
         elif bucket_name is not None:
             b.display_name = bucket_name
         async_bucket_methods = []
         b_from_boto = await loop.run_in_executor(None, s3_resource.Bucket, b.name)
         b.created = creation_date if creation_date else b_from_boto.creation_date
         b.bucket_id = b.name
         b.source = AWS_S3
-        b.region = s3_client.get_bucket_location(Bucket=b.name)['LocationConstraint']
 
         async def _get_version_status(b: AWSBucket):
             logger.debug('Getting version status of bucket %s', b.name)
             try:
                 bucket_versioning = await loop.run_in_executor(None,
                                                                partial(s3_client.get_bucket_versioning, Bucket=b.name))
                 logger.debug('bucket_versioning=%s', bucket_versioning)
@@ -2063,15 +2090,15 @@
 
         async_bucket_methods.append(_get_version_status(b))
 
         async def _get_region(b: AWSBucket):
             logger.debug('Getting region of bucket %s', b.name)
             try:
                 loc = await loop.run_in_executor(None, partial(s3_client.get_bucket_location, Bucket=b.name))
-                b.region = loc['LocationConstraint']
+                b.region = loc['LocationConstraint'] or 'us-east-1'
             except ClientError as ce:
                 logging.exception('Error getting the region of bucket %s', b.name)
                 raise ce
             logger.debug('Got region of bucket %s successfully', b.name)
 
         async_bucket_methods.append(_get_region(b))
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/database.py` & `heaserver-1.0.0a99/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/dbapi2.py` & `heaserver-1.0.0a99/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/mongo.py` & `heaserver-1.0.0a99/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.0.0a99/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.0.0a99/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/functional.py` & `heaserver-1.0.0a99/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.0.0a99/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/jsonschema.py` & `heaserver-1.0.0a99/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/jsonschemas/cjtemplate.json` & `heaserver-1.0.0a99/src/heaserver/service/jsonschemas/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/jsonschemas/wstl.json` & `heaserver-1.0.0a99/src/heaserver/service/jsonschemas/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/jsonschemas/wstlaction.json` & `heaserver-1.0.0a99/src/heaserver/service/jsonschemas/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.0.0a99/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/messagebroker.py` & `heaserver-1.0.0a99/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/mimetypes.py` & `heaserver-1.0.0a99/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.0.0a99/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/openapi.py` & `heaserver-1.0.0a99/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/__init__.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/cj.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/factory.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/representor.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/wstljson.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.0.0a99/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/response.py` & `heaserver-1.0.0a99/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/runner.py` & `heaserver-1.0.0a99/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/collection.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/docker.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/expectedvalues.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,19 +15,60 @@
 from enum import Enum
 from heaobject.root import is_primitive, is_primitive_list, is_heaobject_dict_list, is_heaobject_dict, HEAObjectDict, \
     Primitive, HEAObjectDictValue, MemberObjectDict, Union, DesktopObjectDict
 from datetime import date, time
 from heaserver.service.representor.cj import add_extended_property_values
 
 
-@dataclass
 class Action:
-    name: str
-    rel: Optional[List[str]] = None
-    url: Optional[str] = None
+    def __init__(self, name: str, rel: list[str] | None = None, url: str | None = None, wstl_url: str | None = None):
+        self.__name = name
+        self.__rel = list(rel) if rel is not None else None
+        self.__url = url
+        if wstl_url is not None:
+            self.__wstl_url = wstl_url
+        else:
+            self.__wstl_url = url
+
+    @property
+    def name(self) -> str:
+        return self.__name
+
+    @name.setter
+    def name(self, name: str):
+        self.__name = str(name)
+
+    @property
+    def rel(self) -> list[str] | None:
+        return list(self.__rel)
+
+    @rel.setter
+    def rel(self, rel: list[str] | None):
+        if rel is not None:
+            self.__rel = list(rel)
+        else:
+            self.__rel = None
+
+    @property
+    def url(self) -> str:
+        return self.__url
+
+    @url.setter
+    def url(self, url: str):
+        self.__url = str(url)
+        if url is not None and self.wstl_url is None:
+            self.wstl_url = str(url)
+
+    @property
+    def wstl_url(self) -> str | None:
+        return self.__wstl_url
+
+    @wstl_url.setter
+    def wstl_url(self, wstl_url: str | None):
+        self.__wstl_url = str(wstl_url)
 
 
 @dataclass
 class Link:
     url: str
     rel: Optional[List[str]]
 
@@ -87,15 +128,15 @@
     :param get_actions: the actions to include in the body of GET calls.
     :return: a run-time WeSTL document as a dict.
     """
     if get_actions is None:
         get_actions = []
     actions = []
     href_ = wstl_builder.href if wstl_builder.href else ''
-    for action, action_name, action_rel, action_url in ((wstl_builder.find_action(a.name), a.name, a.rel, a.url) for a
+    for action, action_name, action_rel, action_url in ((wstl_builder.find_action(a.name), a.name, a.rel, a.wstl_url) for a
                                                         in get_actions):
         if action is None:
             raise ValueError(f'No action with name {action_name}')
         for input in action.get('inputs', []):
             if optionsFromUrl := wstl.get_extended_property_value('optionsFromUrl', input):
                 optionsFromUrl['href'] = 'http://localhost:8080' + optionsFromUrl.get('path', '')
         if action is None:
@@ -334,15 +375,15 @@
     if get_all_actions is None:
         get_all_actions = []
 
     href_ = wstl_builder.href if wstl_builder.href else ''
 
     def runtime_actions():
         result = []
-        for action, action_name, action_rel, action_url in ((wstl_builder.find_action(a.name), a.name, a.rel, a.url) for
+        for action, action_name, action_rel, action_url in ((wstl_builder.find_action(a.name), a.name, a.rel, a.wstl_url) for
                                                             a in get_all_actions):
             if action is None:
                 raise ValueError(f'Action {action_name} does not exist')
             href = action_url if action_url else 'http://localhost:8080'
             action['href'] = href
             action['rel'] = action_rel if action_rel else []
             for input in action.get('inputs', []):
@@ -470,15 +511,16 @@
                     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
                     duplicate_action_name: str | None,
                     href: Optional[Union[str, URL]],
                     get_actions: Optional[List[Action]] = None,
                     get_all_actions: Optional[List[Action]] = None,
                     opener_link: Optional[Link] = None,
                     default_db_manager_cls: Type[MicroserviceDatabaseManager] = MicroserviceDatabaseManager,
-                    duplicate_action_actions: list[Action] | None = None) -> Dict[str, Any]:
+                    duplicate_action_actions: list[Action] | None = None,
+                    exclude: list[str] | None = None) -> Dict[str, Any]:
     """
     Generate a dict of all the expected values for passing into the mongotestcase and mockmongotestcase
     get_test_case_cls function.
 
     :param fixtures: the data to load into the database, as a map of collection name -> list of desktop object dicts.
     Required.
     :param coll: the collection name to use. Required.
@@ -491,34 +533,44 @@
     :param default_db_manager_cls: The database manager to use if the collection key is a string. Defaults to
     DatabaseManager.
     :return: a dict of keyword argument name -> Collection+JSON dict or WeSTL document dict, where the keyword arguments
     match those of the mongotestcase and mockmongotestcase get_test_case_cls functions.
     """
     wstl_builder_ = copy.deepcopy(wstl_builder)
     wstl_builder_.href = str(href) if href is not None else None
-    body_put_ = body_put(fixtures, coll, default_db_manager_cls)
-    content_id = next((e.get('value') for e in body_put_['template']['data'] if e['name'] == 'id'), None)
-    return {
-        'body_post': body_post(fixtures, coll, default_db_manager_cls),
-        'body_put': body_put_,
-        'content_id': content_id,
-        'expected_one_wstl': expected_one_wstl(fixtures, coll, wstl_builder_, default_db_manager_cls,
-                                               get_actions=get_actions),
-        'expected_one': expected_one(fixtures, coll, wstl_builder_, default_db_manager_cls, get_actions=get_actions),
-        'expected_one_duplicate_form': expected_one_duplicate_form(fixtures, coll, wstl_builder_,
+    result = {}
+    if not exclude or ('body_put' not in exclude):
+        body_put_ = body_put(fixtures, coll, default_db_manager_cls)
+        content_id = next((e.get('value') for e in body_put_['template']['data'] if e['name'] == 'id'), None)
+        result['body_put'] = body_put_
+        result['content_id'] = content_id
+    if not exclude or ('body_post' not in exclude):
+        result['body_post'] = body_post(fixtures, coll, default_db_manager_cls)
+    if not exclude or ('expected_one_wstl' not in exclude):
+        result['expected_one_wstl'] = expected_one_wstl(fixtures, coll, wstl_builder_, default_db_manager_cls,
+                                                        get_actions=get_actions)
+    if not exclude or ('expected_one' not in exclude):
+        result['expected_one'] = expected_one(fixtures, coll, wstl_builder_, default_db_manager_cls,
+                                              get_actions=get_actions)
+    if not exclude or ('expected_one_duplicate_form' not in exclude):
+        result['expected_one_duplicate_form'] = expected_one_duplicate_form(fixtures, coll, wstl_builder_,
                                                                    default_db_manager_cls, duplicate_action_name,
-                                                                   actions=duplicate_action_actions),
-        'expected_all_wstl': expected_all_wstl(fixtures, coll, wstl_builder_, default_db_manager_cls,
-                                               get_all_actions=get_all_actions),
-        'expected_all': expected_all(fixtures, coll, wstl_builder_, default_db_manager_cls,
-                                     get_all_actions=get_all_actions),
-        'expected_opener': opener_link.url if opener_link is not None else None,
-        'expected_opener_body': expected_opener_body(fixtures, coll, wstl_builder_, default_db_manager_cls,
+                                                                   actions=duplicate_action_actions)
+    if not exclude or ('expected_all_wstl' not in exclude):
+        result['expected_all_wstl'] = expected_all_wstl(fixtures, coll, wstl_builder_, default_db_manager_cls,
+                                               get_all_actions=get_all_actions)
+    if not exclude or ('expected_all' not in exclude):
+        result['expected_all'] = expected_all(fixtures, coll, wstl_builder_, default_db_manager_cls,
+                                     get_all_actions=get_all_actions)
+    if not exclude or ('expected_opener' not in exclude):
+        result['expected_opener'] = opener_link.url if opener_link is not None else None
+    if not exclude or ('expected_opener_body' not in exclude):
+        result['expected_opener_body'] = expected_opener_body(fixtures, coll, wstl_builder_, default_db_manager_cls,
                                                      get_actions=get_actions, opener_link=opener_link)
-    }
+    return result
 
 
 def _create_template(d: DesktopObjectDict, exclude=('id',)) -> Dict[str, Dict[str, List[Dict[str, Any]]]]:
     return {'template': {'data': [z for x, y in d.items() if (not exclude or x not in exclude) for z in
                                   _nvpjson_property_to_cj_part_generator(x, y)]}}
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,16 +206,16 @@
     coll_ = coll if isinstance(coll, CollectionKey) else CollectionKey(name=coll, db_manager_cls=db_manager_cls)
     expected_values_ = {k: v for k, v in expected_values(fixtures, coll_, wstl.builder(package=wstl_package),
                                                          duplicate_action_name, href,
                                                          get_actions=get_actions,
                                                          get_all_actions=get_all_actions,
                                                          opener_link=expected_opener,
                                                          default_db_manager_cls=db_manager_cls,
-                                                         duplicate_action_actions=duplicate_action_actions).items()
-                        if k not in exclude_ and v is not None}
+                                                         duplicate_action_actions=duplicate_action_actions,
+                                                         exclude=exclude_).items() if v is not None}
 
     class ExpectedValuesMicroserviceTestCase(MicroserviceTestCase):
         def __init__(self, methodName: str = 'runTest') -> None:
             super().__init__(coll=coll, desktop_objects=fixtures, db_manager_cls=db_manager_cls,
                              wstl_package=wstl_package, href=href, content=content, content_type=content_type,
                              put_content_status=put_content_status, registry_docker_image=registry_docker_image,
                              other_docker_images=other_docker_images, port=port, sub=sub, methodName=methodName,
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/mixin.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/mockaws.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,19 @@
         else:
             creds = self._get_credential_by_volume(volume_id=volume_id)
         return AWSFileSystem(), creds
 
     async def get_volumes(self, request: Request, file_system_type_or_type_name: Union[str, type[FileSystem]]) -> \
         AsyncGenerator[Volume, None]:
         for volume_dict in self.get_desktop_objects_by_collection('volumes'):
-            if isinstance(file_system_type_or_type_name, DesktopObject):
-                file_system_type_or_type_name_ = file_system_type_or_type_name.get_type_name()
+            if issubclass(file_system_type_or_type_name, DesktopObject):
+                file_system_type_name_ = file_system_type_or_type_name.get_type_name()
             else:
-                file_system_type_or_type_name_ = str(file_system_type_or_type_name)
-            if volume_dict.get('file_system_type', DEFAULT_FILE_SYSTEM) == file_system_type_or_type_name_:
+                file_system_type_name_ = str(file_system_type_or_type_name)
+            if volume_dict.get('file_system_type', AWSFileSystem.get_type_name()) == file_system_type_name_:
                 volume = Volume()
                 volume.from_dict(volume_dict)
                 yield volume
 
     async def get_property(self, app: web.Application, name: str) -> Optional[Property]:
         prop_dict_list = [prop_dict for prop_dict in self.get_desktop_objects_by_collection('properties')
                           if prop_dict.get('name', None) == name]
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/testcase/testenv.py` & `heaserver-1.0.0a99/src/heaserver/service/testcase/testenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from heaserver.service.db.database import MicroserviceDatabaseManager
 from heaserver.service.testcase.collection import query_fixtures, query_content, CollectionKey, \
     get_collection_key_from_name
 from heaserver.service.testcase.mockmongo import MockMongoManager
 from contextlib import contextmanager, closing
 from collections.abc import Generator
 from abc import ABC
+from ..util import retry
 import logging
+from concurrent.futures import ThreadPoolExecutor
 
 
 class DockerVolumeMapping:
     """
     Docker volume mapping. This class is immutable.
     """
 
@@ -343,17 +345,22 @@
             bridge_db_manager_cls.update(
                 [img.db_manager_cls for img in other_docker_images if
                  isinstance(img, MicroserviceContainerConfig) and img.db_manager_cls is not None])
         if registry_docker_image is not None and registry_docker_image.db_manager_cls is not None:
             bridge_db_manager_cls.add(registry_docker_image.db_manager_cls)
         return bridge_db_manager_cls
 
-    with ExitStack() as context_manager, closing(
-        db_manager_cls()) as external_db_, db_manager_cls.environment(), db_manager_cls.context():
-        from concurrent.futures import ThreadPoolExecutor
+    class TestEnvExitStack(ExitStack):
+        @retry(ValueError, retries=3, cooldown=10)
+        def __exit__(self, exc_type, exc_val, exc_tb) -> bool:
+            return super().__exit__(exc_type, exc_val, exc_tb)
+
+    with TestEnvExitStack() as context_manager, closing(db_manager_cls()) as external_db_, \
+        db_manager_cls.environment(), db_manager_cls.context():
+
         with ThreadPoolExecutor() as pool:
             bridge_dbs = [context_manager.enter_context(closing(bridge_db_cls())) for bridge_db_cls in
                           _bridge_dbs_to_start()]
             bridge_desktop_objects, external_desktop_objects = dict(deepcopy(desktop_objects)), dict(
                 deepcopy(desktop_objects))
             external_db_.start_database(context_manager)
             if registry_docker_image is not None:
```

### Comparing `heaserver-1.0.0a98/src/heaserver/service/uritemplate.py` & `heaserver-1.0.0a99/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/util.py` & `heaserver-1.0.0a99/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver/service/wstl.py` & `heaserver-1.0.0a99/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.0.0a99/src/heaserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.0.0a98
+Version: 1.0.0a99
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `heaserver-1.0.0a98/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.0.0a99/src/heaserver.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 src/heaserver/service/appfactory.py
 src/heaserver/service/appproperty.py
 src/heaserver/service/caching.py
 src/heaserver/service/caching_strategy.py
 src/heaserver/service/client.py
 src/heaserver/service/config.py
 src/heaserver/service/defaults.py
+src/heaserver/service/expression.py
 src/heaserver/service/functional.py
 src/heaserver/service/heaobjectsupport.py
 src/heaserver/service/jsonschema.py
 src/heaserver/service/jsonschemavalidator.py
 src/heaserver/service/messagebroker.py
 src/heaserver/service/mimetypes.py
 src/heaserver/service/oidcclaimhdrs.py
@@ -107,14 +108,15 @@
 tests/heaserver/servicetest/organizationtestcase.py
 tests/heaserver/servicetest/service.py
 tests/heaserver/servicetest/test_caching.py
 tests/heaserver/servicetest/test_client.py
 tests/heaserver/servicetest/test_component_with_bad_permissions.py
 tests/heaserver/servicetest/test_configuration.py
 tests/heaserver/servicetest/test_delete_component.py
+tests/heaserver/servicetest/test_expression.py
 tests/heaserver/servicetest/test_functional.py
 tests/heaserver/servicetest/test_get_all_components.py
 tests/heaserver/servicetest/test_get_component.py
 tests/heaserver/servicetest/test_get_organization_permissions.py
 tests/heaserver/servicetest/test_heaobjectsupport.py
 tests/heaserver/servicetest/test_jsonschemavalidator.py
 tests/heaserver/servicetest/test_organization_with_bad_permissions.py
```

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/service.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_client.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_response.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_util.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.0.0a99/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.0.0a98/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.0.0a99/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

