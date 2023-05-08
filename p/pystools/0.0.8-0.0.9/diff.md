# Comparing `tmp/pystools-0.0.8.tar.gz` & `tmp/pystools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystools-0.0.8.tar", last modified: Wed Apr 26 09:04:53 2023, max compression
+gzip compressed data, was "pystools-0.0.9.tar", last modified: Tue May  2 03:29:17 2023, max compression
```

## Comparing `pystools-0.0.8.tar` & `pystools-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.473257 pystools-0.0.8/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-16 08:21:09.000000 pystools-0.0.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 09:04:53.471766 pystools-0.0.8/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      106 2023-04-26 05:41:53.000000 pystools-0.0.8/README.md
--rw-r--r--   0 steve      (501) staff       (20)      602 2023-04-26 09:04:32.000000 pystools-0.0.8/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 09:04:53.473528 pystools-0.0.8/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.457816 pystools-0.0.8/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.460207 pystools-0.0.8/src/PysTools.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      583 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      709 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       18 2023-04-26 09:04:53.000000 pystools-0.0.8/src/PysTools.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)        2 2023-04-26 03:57:58.000000 pystools-0.0.8/src/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.468411 pystools-0.0.8/src/pystools/
--rw-r--r--   0 steve      (501) staff       (20)     1278 2023-04-26 04:59:47.000000 pystools-0.0.8/src/pystools/BizResponse.py
--rw-r--r--   0 steve      (501) staff       (20)      537 2023-04-26 04:59:15.000000 pystools-0.0.8/src/pystools/BizResponseCode.py
--rwxr-xr-x   0 steve      (501) staff       (20)    28074 2023-04-26 09:03:30.000000 pystools-0.0.8/src/pystools/Feishu.py
--rw-r--r--   0 steve      (501) staff       (20)     1454 2023-04-26 05:07:11.000000 pystools-0.0.8/src/pystools/Jwt.py
--rw-r--r--   0 steve      (501) staff       (20)     1876 2023-04-26 05:34:33.000000 pystools-0.0.8/src/pystools/LexinSms.py
--rw-r--r--   0 steve      (501) staff       (20)     1535 2023-04-25 17:01:25.000000 pystools-0.0.8/src/pystools/Logger.py
--rw-r--r--   0 steve      (501) staff       (20)      259 2023-04-26 05:25:35.000000 pystools-0.0.8/src/pystools/MD5util.py
--rw-r--r--   0 steve      (501) staff       (20)     4013 2023-04-26 06:12:55.000000 pystools-0.0.8/src/pystools/TencentCos.py
--rwxr-xr-x   0 steve      (501) staff       (20)     5183 2023-04-26 07:17:47.000000 pystools-0.0.8/src/pystools/Xiumi.py
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 03:57:35.000000 pystools-0.0.8/src/pystools/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-04-16 08:20:17.000000 pystools-0.0.8/src/pystools/example.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-26 09:04:53.470422 pystools-0.0.8/src/pystools/test/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 04:53:20.000000 pystools-0.0.8/src/pystools/test/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-02 03:29:17.738507 pystools-0.0.9/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-16 08:21:09.000000 pystools-0.0.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)      583 2023-05-02 03:29:17.738139 pystools-0.0.9/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      106 2023-04-26 05:41:53.000000 pystools-0.0.9/README.md
+-rw-r--r--   0 steve      (501) staff       (20)      602 2023-05-02 03:27:40.000000 pystools-0.0.9/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-02 03:29:17.738623 pystools-0.0.9/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-02 03:29:17.730609 pystools-0.0.9/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-02 03:29:17.732396 pystools-0.0.9/src/PysTools.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      583 2023-05-02 03:29:17.000000 pystools-0.0.9/src/PysTools.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      709 2023-05-02 03:29:17.000000 pystools-0.0.9/src/PysTools.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-02 03:29:17.000000 pystools-0.0.9/src/PysTools.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-02 03:29:17.000000 pystools-0.0.9/src/PysTools.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       18 2023-05-02 03:29:17.000000 pystools-0.0.9/src/PysTools.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)        2 2023-04-26 03:57:58.000000 pystools-0.0.9/src/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-02 03:29:17.736820 pystools-0.0.9/src/pystools/
+-rw-r--r--   0 steve      (501) staff       (20)     1278 2023-04-26 04:59:47.000000 pystools-0.0.9/src/pystools/BizResponse.py
+-rw-r--r--   0 steve      (501) staff       (20)      537 2023-04-26 04:59:15.000000 pystools-0.0.9/src/pystools/BizResponseCode.py
+-rwxr-xr-x   0 steve      (501) staff       (20)    28358 2023-05-02 03:28:53.000000 pystools-0.0.9/src/pystools/Feishu.py
+-rw-r--r--   0 steve      (501) staff       (20)     1454 2023-04-26 05:07:11.000000 pystools-0.0.9/src/pystools/Jwt.py
+-rw-r--r--   0 steve      (501) staff       (20)     1876 2023-04-26 05:34:33.000000 pystools-0.0.9/src/pystools/LexinSms.py
+-rw-r--r--   0 steve      (501) staff       (20)     1535 2023-04-25 17:01:25.000000 pystools-0.0.9/src/pystools/Logger.py
+-rw-r--r--   0 steve      (501) staff       (20)      259 2023-04-26 05:25:35.000000 pystools-0.0.9/src/pystools/MD5util.py
+-rw-r--r--   0 steve      (501) staff       (20)     7119 2023-05-02 03:25:57.000000 pystools-0.0.9/src/pystools/TencentCos.py
+-rwxr-xr-x   0 steve      (501) staff       (20)     5183 2023-04-26 07:17:47.000000 pystools-0.0.9/src/pystools/Xiumi.py
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 03:57:35.000000 pystools-0.0.9/src/pystools/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-04-16 08:20:17.000000 pystools-0.0.9/src/pystools/example.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-02 03:29:17.737714 pystools-0.0.9/src/pystools/test/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-26 04:53:20.000000 pystools-0.0.9/src/pystools/test/__init__.py
```

### Comparing `pystools-0.0.8/PKG-INFO` & `pystools-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystools
-Version: 0.0.8
+Version: 0.0.9
 Summary: pystools
 Author-email: 木坦坦 <devzhao@126.com>
 Project-URL: Homepage, https://github.com/devzhaohan/HMTools
 Project-URL: Bug Tracker, https://github.com/devzhaohan/HMTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pystools-0.0.8/pyproject.toml` & `pystools-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pystools"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="木坦坦", email="devzhao@126.com" },
 ]
 description = "pystools"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pystools-0.0.8/src/PysTools.egg-info/PKG-INFO` & `pystools-0.0.9/src/PysTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystools
-Version: 0.0.8
+Version: 0.0.9
 Summary: pystools
 Author-email: 木坦坦 <devzhao@126.com>
 Project-URL: Homepage, https://github.com/devzhaohan/HMTools
 Project-URL: Bug Tracker, https://github.com/devzhaohan/HMTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pystools-0.0.8/src/PysTools.egg-info/SOURCES.txt` & `pystools-0.0.9/src/PysTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/BizResponse.py` & `pystools-0.0.9/src/pystools/BizResponse.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/BizResponseCode.py` & `pystools-0.0.9/src/pystools/BizResponseCode.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/Feishu.py` & `pystools-0.0.9/src/pystools/Feishu.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,15 @@
 
 # 将用户或机器人拉入群聊
 chat_members = '/open-apis/im/v1/chats/:chat_id/members'
 
 # 多维表格列出字段
 TABLES_FIELDS = '/open-apis/bitable/v1/apps/:app_token/tables/:table_id/fields'
 
-lark_host="https://open.feishu.cn"
-
+lark_host = "https://open.feishu.cn"
 
 
 class Feishu(object):
     def __init__(self, app_id, app_secret,
                  print_feishu_log=True, logger=Loggings()):
 
         """
@@ -95,16 +94,14 @@
         self.logger = logger
         self._tenant_access_token = ""
 
         self._app_id = app_id
         self._app_secret = app_secret
         self.print_feishu_log = print_feishu_log
 
-
-
     @property
     def tenant_access_token(self):
         return self._tenant_access_token
 
     def _authorize_tenant_access_token(self):
         # get tenant_access_token and set, implemented based on Feishu open api capability. doc link: https://open.feishu.cn/document/ukTMukTMukTM/ukDNz4SO0MjL5QzM/auth-v3/auth/tenant_access_token_internal
         url = "{}{}".format(lark_host, TENANT_ACCESS_TOKEN_URI)
@@ -119,24 +116,25 @@
             if resp.status != 200:
                 try:
                     response_dict = json.loads(resp.data.decode('utf-8'))
                     raise LarkException(code=response_dict.get("code", -1), msg=resp.data.decode('utf-8'), url=url,
                                         req_body=req_body, headers=headers)
                 except:
                     raise LarkException(code=resp.status, msg="response status: {}  ,response data: {} ".format(
-                        resp.status,resp.data.decode('utf-8')),
+                        resp.status, resp.data.decode('utf-8')),
                                         url=url,
                                         req_body=req_body, headers=headers)
         # response_dict = resp.json()
         if check_code:
             response_dict = json.loads(resp.data.decode('utf-8'))
             code = response_dict.get("code", -1)
             if code != 0:
                 self.logger.exception("url:{},response:{}".format(url, response_dict))
-                raise LarkException(code=code, msg=response_dict.get("msg"), url=url, req_body=req_body, headers=headers)
+                raise LarkException(code=code, msg=response_dict.get("msg"), url=url, req_body=req_body,
+                                    headers=headers)
 
     def _handle_resp_code(self, resp, req_url):
         try:
             response_dict = json.loads(resp.data.decode('utf-8'))
             code = response_dict.get("code")
             if code != 0:
                 msg_type = 'post'
@@ -146,15 +144,16 @@
                         "content": [
                             [{
                                 "tag": "text",
                                 "text": '请求接口: {}\n'.format(req_url)
                             },
                                 {
                                     "tag": "text",
-                                    "text": '返回异常: {} \n'.format(json.dumps(response_dict, ensure_ascii=False, indent=4, separators=(',', ': ')))
+                                    "text": '返回异常: {} \n'.format(
+                                        json.dumps(response_dict, ensure_ascii=False, indent=4, separators=(',', ': ')))
                                 }
                             ],
                             [{
                                 "tag": "text",
                                 "text": "使用方法见 :\n"
                             }, {
                                 "tag": "a",
@@ -192,27 +191,28 @@
             if 'attachment' in Content_Disposition:
                 if str(content_type).__contains__("json"):
                     resp_msg = resp.data.decode('utf-8')
                     try:
                         resp_dict = json.loads(resp_msg)
                     except:
                         return {'content_type': content_type, 'file_bytes': resp_data}
-                    code = resp_dict.get("code",None)
+                    code = resp_dict.get("code", None)
                     msg = resp_dict.get("msg", None)
                     error = resp_dict.get("error", None)
                     if code and msg and error:
-                        raise LarkException(code=code, msg=json.dumps(resp_dict,ensure_ascii=False), url=url,req_body=req_body, headers=headers)
+                        raise LarkException(code=code, msg=json.dumps(resp_dict, ensure_ascii=False), url=url,
+                                            req_body=req_body, headers=headers)
 
-                return {'content_type':content_type,'file_bytes':resp_data}
+                return {'content_type': content_type, 'file_bytes': resp_data}
 
         resp_msg = resp.data.decode('utf-8')
         if self.print_feishu_log:
             self.logger.info("飞书接口响应：{}".format(resp_msg))
 
-        self._check_error_response(resp, check_code, check_status, unquote(url),headers)
+        self._check_error_response(resp, check_code, check_status, unquote(url), headers)
         try:
             response_dict = json.loads(resp_msg)
             return response_dict
         except:
             return resp_msg
 
         # # resp.release_conn()
@@ -265,25 +265,23 @@
             if req_body:
                 action = "PUT"
         if param:
             url = url + "?" + urlencode(param)
         resp = self.req_feishu_api(action, url=url, req_body=req_body)
         return resp.get("data")
 
-
     def bitable_record_delete(self, file_token, table_id, record_id):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, BITABLE_RECORD
         ).replace(":app_token", file_token).replace(":table_id", table_id).replace(":record_id", record_id)
         action = "DELETE"
         resp = self.req_feishu_api(action, url=url)
         return resp.get("data")
 
-
     def bitable_record(self, file_token, table_id, record_id):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, BITABLE_RECORD
         ).replace(":app_token", file_token).replace(":table_id", table_id).replace(":record_id", record_id)
         action = "GET"
         resp = self.req_feishu_api(action, url=url)
@@ -294,16 +292,14 @@
         file_bytes = file_res.get("file_bytes")
 
         subfix = file_res.get("content_type").split("/")[1]
         filename = file_token + "." + subfix
 
         return filename, file_bytes
 
-
-
     def medias_download_to_bytes(self, file_token, param={}):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, MEDIAS_DOWNLOAD
         ).replace(":file_token", file_token)
         if param:
             url = url + "?" + urlencode(param)
@@ -315,19 +311,18 @@
 
     def medias_batch_get_tmp_download_url(self, file_tokens):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, MEDIAS_BATCH_GET_TMP_DOWNLOAD_URL
         )
 
-        url = url + "?" + urlencode({"file_tokens":file_tokens})
+        url = url + "?" + urlencode({"file_tokens": file_tokens})
         resp = self.req_feishu_api("GET", url=url, check_code=False)
         return resp.get("data")
 
-
     def drive_files_download_to_bytes(self, file_token):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, DRIVE_FILES_DOWNLOAD
         ).replace(":file_token", file_token)
         resp = self.req_feishu_api("GET", url=url, check_code=False)
         content_type = resp.get("content_type")
@@ -464,18 +459,20 @@
         elif type(file_path_or_binary) is str:
             if os.path.isfile(file_path_or_binary):
                 file_size = os.path.getsize(file_path_or_binary)
                 # file_binary = (open(file_path_or_binary, 'rb'))  #BufferedReader
                 with open(file_path_or_binary, 'rb') as f:
                     file_binary = f.read()  # bytes
             else:
-                raise LarkException(code=-1, msg="file_path_or_binary参数：{} 应该是文件路径".format(file_path_or_binary),
+                raise LarkException(code=-1,
+                                    msg="file_path_or_binary参数：{} 应该是文件路径".format(file_path_or_binary),
                                     url=url)
         else:
-            raise LarkException(code=-1, msg="file_path_or_binary参数：{} 应该是文件路径或bytes".format(file_path_or_binary),
+            raise LarkException(code=-1,
+                                msg="file_path_or_binary参数：{} 应该是文件路径或bytes".format(file_path_or_binary),
                                 url=url)
 
         form = {'file_name': file_name,
                 'parent_type': parent_type,
                 'parent_node': parent_node,
                 'size': str(file_size),
                 'file': file_binary
@@ -549,16 +546,15 @@
         #     if member_id == bot_info.get('open_id') and member_perm == perm:
         #         return True
         # return False
 
         # 目前不支持获取机器人类别的协作者，只能用如下方法了
         return self.drive_permission_member_permitted(token, type)
 
-
-    def drive_permission_member_permitted(self,token, type, perm='edit'):
+    def drive_permission_member_permitted(self, token, type, perm='edit'):
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, DRIVE_PERMISSION_MEMBER_PERMITTED
         )
 
         req_body = {
             "token": token,
@@ -574,16 +570,16 @@
         """
         :param token: 文件的 token
         :param type:文档类型，可选 doc、docx、sheet、bitable、file
         :return:
         """
         self._authorize_tenant_access_token()
         url = "{}{}?type={}&fields=*".format(
-            lark_host, DRIVE_PERMISSIONS_MEMBERS,type
-        ).replace(':token',token)
+            lark_host, DRIVE_PERMISSIONS_MEMBERS, type
+        ).replace(':token', token)
         action = "GET"
         resp = self.req_feishu_api(action, url=url)
 
         return resp.get("data")
 
     def notify_send(self, msg_type, msg, receive_id_type, receive_id):
         """
@@ -644,27 +640,25 @@
         url = "{}{}?file_type={}".format(
             lark_host, FILES_SUBSCRIBE, file_type
         ).replace(':file_token', file_token)
         action = "POST"
         resp = self.req_feishu_api(action, url=url, check_code=False, check_status=False)
         return resp
 
-
     def tables_fields(self, app_token, table_id):
 
         self._authorize_tenant_access_token()
         url = "{}{}".format(
             lark_host, TABLES_FIELDS
         ).replace(':app_token', app_token).replace(':table_id', table_id)
         action = "GET"
         resp = self.req_feishu_api(action, url=url)
         return resp.get('data')
 
-
-    def update_bitable_record(self,file_token, table_id, update_data, record_id=None):
+    def update_bitable_record(self, file_token, table_id, update_data, record_id=None):
         """
         更新多维表格的数据
         :param feishu:
         :param file_token:
         :param table_id:
         :param update_data: 格式如 [('(A)状态', "处理中"), ('(A)结果', "正在处理")]
         :param record_id: 如果不传，就是新增一条数据
@@ -679,16 +673,17 @@
         }
         # 将update_data里面的数据添加到data里面
         for item in update_data:
             data['fields'][item[0]] = item[1]
         res = self.bitable_records(file_token, table_id, record_id=record_id, req_body=data)
         return res
 
+
 class LarkException(Exception):
-    def __init__(self, code=0, msg=None, url=None, req_body=None,headers=None):
+    def __init__(self, code=0, msg=None, url=None, req_body=None, headers=None):
         self.url = url
         self.req_body = req_body
         self.code = code
         self.msg = msg
         self.headers = headers
 
     def __str__(self) -> str:
@@ -708,13 +703,21 @@
         :param obj:
         :return:
         """
         if isinstance(obj, bytes):
             return str(obj, encoding='utf-8')
         return json.JSONEncoder.default(self, obj)
 
+
 if __name__ == '__main__':
-    feishu = Feishu(app_id="xxx", app_secret="xxx")
-    res = feishu.bitable_record_delete(file_token="xxx",
-                                       table_id="xxx",record_id="xxx")
-    print(res)
+    app_id = "xxx"
+    app_secret = "xxx"
+
+    file_token = "xxx"
+    table_id = "xxx"
+
+    feishu = Feishu(app_id=app_id, app_secret=app_secret)
+    res = feishu.bitable_records(app_token=file_token,
+                                 table_id=table_id)
+    items = res.get('items')
+
```

### Comparing `pystools-0.0.8/src/pystools/Jwt.py` & `pystools-0.0.9/src/pystools/Jwt.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/LexinSms.py` & `pystools-0.0.9/src/pystools/LexinSms.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/Logger.py` & `pystools-0.0.9/src/pystools/Logger.py`

 * *Files identical despite different names*

### Comparing `pystools-0.0.8/src/pystools/Xiumi.py` & `pystools-0.0.9/src/pystools/Xiumi.py`

 * *Files identical despite different names*

