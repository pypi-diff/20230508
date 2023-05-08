# Comparing `tmp/aliyun-python-sdk-cams-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-cams-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.4.tar", last modified: Fri Apr 14 02:21:46 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cams-1.0.5.tar", last modified: Mon May  8 11:47:50 2023, max compression
```

## Comparing `aliyun-python-sdk-cams-1.0.4.tar` & `aliyun-python-sdk-cams-1.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1542 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2342 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/
--rw-r--r--   0 root         (0) root         (0)     2636 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py
--rw-r--r--   0 root         (0) root         (0)     1680 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2044 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2432 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     1493 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1414 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2988 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     4040 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     5334 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2631 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2457 2023-04-14 02:21:46.000000 aliyun-python-sdk-cams-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1434 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1414 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1656 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-05-08 11:47:50.000000 aliyun-python-sdk-cams-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-cams-1.0.4/LICENSE` & `aliyun-python-sdk-cams-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/PKG-INFO` & `aliyun-python-sdk-cams-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.4
+Version: 1.0.5
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.4/README.rst` & `aliyun-python-sdk-cams-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/PKG-INFO` & `aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cams
-Version: 1.0.4
+Version: 1.0.5
 Summary: The cams module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cams
```

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyun_python_sdk_cams.egg-info/SOURCES.txt` & `aliyun-python-sdk-cams-1.0.5/aliyun_python_sdk_cams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/endpoint.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/BeeBotAssociateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/BeeBotChatRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappBindWabaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappEmbedSignUpRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappMigrationRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappMigrationVerifiedRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappPhoneNumberRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappSyncPhoneNumberRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ChatappVerifyAndRegisterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/CreateChatappMigrationInitiateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/CreateChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/DeleteChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappTemplateDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappUploadAuthorizationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetChatappVerifyCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetMigrationVerifyCodeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/GetPhoneNumberVerificationStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/IsvGetAppIdRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ListChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ModifyChatappTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/ModifyPhoneBusinessProfileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryChatappBindWabaRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryChatappPhoneNumbersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryPhoneBusinessProfileRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/QueryWabaBusinessInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SendChatappMassMessageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SendChatappMessageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/SubmitIsvCustomerTermsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/UpdateAccountWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py` & `aliyun-python-sdk-cams-1.0.5/aliyunsdkcams/request/v20200606/UpdatePhoneWebhookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cams-1.0.4/setup.py` & `aliyun-python-sdk-cams-1.0.5/setup.py`

 * *Files identical despite different names*

